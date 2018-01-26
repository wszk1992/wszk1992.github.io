---
title: Markdown Handbook
---
* [Headings](#Headings)
* [Horizontal Rules](#Horizontal-Rules)
* [Inline HTML](#Inline-HTML)
* [Emphasis](#Emphasis)
* [Blockquotes](#Blockquotes)
* [Lists](#Lists)
* [Code](#Code)
* [Table](#Table)
* [Links](#Links)
* [Images](#Images)

# Headings

```
# h1 Heading
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading
```

Renders to:
# h1 Heading
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Headingdfdf
###### h6 Heading

<!--This is a comment-->

# Horizontal Rules
`***`: Three consecutive asterisks for `<hr>`
```
abcd
***
efgh
```
Renders to:
abcd
***
efgh

# Inline HTML
```HTML
<button>button</button>
```
<button>button</button>

# Emphasis
**Bold**: `**Bold**` 
*Italics*: `*Italics*`
~~Strike~~: `~~Strike~~`

# Blockquotes
Add`>`before and text you want to quote
```
> **Edward Christopher** Sheeran, MBE (born 17 February 1991) is an English singer, songwriter, guitarist, and record producer. 
```
Renders to:
> **Edward Christopher** Sheeran, MBE (born 17 February 1991) is an English singer, songwriter, guitarist, and record producer. 

# Lists
#### Unordered
```
* valid bullet
- valid bullet
+ valid bullet
```
```
+ Lorem ipsum dolor sit amet
+ Consectetur adipiscing elit
+ Integer molestie lorem at massa
+ Facilisis in pretium nisl aliquet
+ Nulla volutpat aliquam velit
  - Phasellus iaculis neque
  - Purus sodales ultricies
  - Vestibulum laoreet porttitor sem
  - Ac tristique libero volutpat at
+ Faucibus porta lacus fringilla vel
+ Aenean sit amet erat nunc
+ Eget porttitor lorem
```
Renders to:
+ Lorem ipsum dolor sit amet
+ Consectetur adipiscing elit
+ Integer molestie lorem at massa
+ Facilisis in pretium nisl aliquet
+ Nulla volutpat aliquam velit
  - Phasellus iaculis neque
  - Purus sodales ultricies
  - Vestibulum laoreet porttitor sem
  - Ac tristique libero volutpat at
+ Faucibus porta lacus fringilla vel
+ Aenean sit amet erat nunc
+ Eget porttitor lorem

#### Ordered
```
1. abc
2. efg
3. ijk
```
Renders to:
1. abc
2. efg
3. ijk

# Code
`Inline`: 
```
`Inline`
```

#### Block code "fences"
```
``` markup
Sample text here
``` 
```

``` markup
Sample text here
```

# Table
```
|Name|City|
|:-:|:-:|
|Kan|Hangzhou|
|James|Beijing|
|Davis|Houston|
```
|Name|City|
|:-:|:-:|
|Kan|Hangzhou|
|James|Beijing|
|Davis|Houston|

# Links
```
[BasicLink](https://github.com/wszk1992)
```
Renders to: 
[BasicLink](https://github.com/wszk1992)

```
[Add A Title](https://github.com/wszk1992/ "this is title")
```
Renders to:
[Add A Title](https://github.com/wszk1992/ "this is title")

#### Named Anchors
```
* [Headings](#Headings)
* [Horizontal Rules](#Horizontal-Rules)
* [Blockquotes](#Blockquotes)
* [Code](#Code)
```

* [Headings](#Headings)
* [Horizontal Rules](#Horizontal-Rules)
* [Blockquotes](#Blockquotes)
* [Code](#Code)

# Images
```
![alberteinste](https://3c1703fe8d.site.internapcdn.net/newman/csz/news/800/2015/alberteinste.jpg)
```
![alberteinste](https://3c1703fe8d.site.internapcdn.net/newman/csz/news/800/2015/alberteinste.jpg)

