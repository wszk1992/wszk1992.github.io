---
title: Elastic Beanstalk worker & SQS
---

# What is Elastic beanstalk worker?
Worker will received the data from SQS when some visible data is in the queue by the way of http post  through specific endpoint, which can be set when environment is created and configured latter.
https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/using-features-managing-env-tiers.html

# What is SQS?
SQS (simple queue service) is a AWS service, which can received data and put them in the queue as well as wait for some other application or worker to consume the data.
https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/Welcome.html

# SQS SDKs:
send msg to queue:
```java
String queue_url = this.sqs.getQueueUrl(ConfigManager.QUEUE_NAME).getQueueUrl();
Map<String, MessageAttributeValue> attrs;
SendMessageRequest send_msg_request = new SendMessageRequest()
        .withQueueUrl(queue_url)
        .withMessageBody(body)
        .withMessageAttributes(attrs)
        .withDelaySeconds(messageDelay);
SendMessageResult res = sqs.sendMessage(send_msg_request);
return res;
```

Worker side code to receive data from queue:
```java
@RequestMapping(method = RequestMethod.POST, value = "/erpWorker")
public Object erpWorker(@RequestHeader Map<String, MessageAttributeValue> attrs, @RequestBody OrderInfoModel item) {
    //customized attr with name: isReverse 
    Boolean isReverseBoolean = attrs.containsKey("X-Aws-Sqsd-Attr-isReverse") && attrs.get("X-Aws-Sqsd-Attr-isReverse").getStringValue().equals("1");
    //do something...
}
```