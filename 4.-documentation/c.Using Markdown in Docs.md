# Using Markdown# 

All docs and text files in Stoplight exist as markdown files. you can edit and customize these files according to your need. This guide will teach you how. 

## [What is Markdown?](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#what-is-markdown)

Markdown is a text-to-HTML conversion tool for web writers.Markdown allows you to write using an easy-to-read, easy-to-write plain text format, then convert it to structurally valid XHTML (or HTML).

> **Note:** For example: This entire page was created using Markdown!

Below is a quick reference of all the Markdown syntax that is supported by Stoplight.

*All of the notes, descriptions, and content fields in the Stoplight editors support use of [Stoplight Flavored Markdown](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd). SMD extends CommonMark adding more advanced features like themable callouts and embedded JSON Schema models.*

### **[Table of Contents](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#table-of-contents)**

- [Headers](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#headers)
- [Emphasis](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#emphasis)
- [Lists](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#lists)
- [Images](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#images)
- [Code and Syntax Highlighting](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#code-and-syntax-highlighting)
- [Tables](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#tables)
- [Blockquotes](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#blockquotes)
- [Inline HTML](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#inline-html)
- [Horizontal Rule](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#horizontal-rule)
- [Line Breaks](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#line-breaks)
- [Videos](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#videos)

## **[Headers](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#headers)**

```
# H1
## H2
### H3
#### H4
##### H5
###### H6

```

# **H1**

## **[H2](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#h2)**

### **[H3](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#h3)**

### **[H4](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#h4)**

### **H5**

### **H6**

## **[Emphasis](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#emphasis)**

```
Emphasis, aka italics, with*asterisks* or_underscores_.
Strong emphasis, aka bold, with **asterisks** or __underscores__.
Combined emphasis with **asterisks and_underscores_**.
Strikethrough uses two tildes. ~~Scratch this.~~

```

Emphasis, aka italics, with *asterisks* or *underscores*.

Strong emphasis, aka bold, with **asterisks** or **underscores**.

Combined emphasis with **asterisks and *underscores***.

Strikethrough uses two tildes. ~~Scratch this.~~

## **[Lists](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#lists)**

> In this example, leading and trailing spaces are shown with with dots: ⋅⋅⋅
> 

```
1. First ordered list item
2. Another item
   ⋅⋅- Unordered sub-list
3. Actual numbers don't matter, just that it's a number
   ⋅⋅1. Ordered sub-list
4. And another item
⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

```

1. First ordered list item
2. Another item
    - Unordered sub-list
3. Actual numbers don't matter, just that it's a number
    1. Ordered sub-list
4. And another item
    
    You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).
    

## **[Links](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#links)**

```
There are two ways to create links:
[I'm a basic link](https://www.google.com)
[Hover over me to see my link title](https://www.google.com "Google's Homepage")
[I'm a relative link to the ./03a-stoplight-flavored-markdown.md file](./03a-stoplight-flavored-markdown.md)

```

There are two ways to create links:

[I'm a basic link](https://www.google.com/)

[Hover over me to see my link title](https://www.google.com/)

[I'm a relative link to the ./03a-stoplight-flavored-markdown.md file](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd)

## **[Images](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#images)**

```
Here's our logo (hover to see the title text):
![Stoplight Logo](https://stoplight.io/images/home/logo-blue-black.png "Stoplight Logo")

```

Here's our logo (hover to see the title text):

![https://stoplight.io/images/home/logo-blue-black.png](https://stoplight.io/images/home/logo-blue-black.png)

Stoplight Logo

To customize images like adding backgrounds, captions or focus, check out [images in Stoplight Flavored Markdown](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd).

## **[Code and Syntax Highlighting](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#code-and-syntax-highlighting)**

Inline **`code`** has **`back-ticks`** around it.

Blocks of code are either fenced by lines with three back-ticks, or are indented with four spaces. We recommend only using the fenced code blocks -- they're easier to use and support syntax highlighting.

> In the examples below, remove the \ that precedes the three backticks at the start and end of the javascript code fence before using.

**untitled**

**javascript**

`\```javascriptvar s = "JavaScript syntax highlighting";alert(s);\````

Use language tags to change the syntax highlighting:

**untitled**

**json**

`\```json{  "JSON": "Syntax Highlighting"}\````

## **[Tables](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#tables)**

```
Colons can be used to align columns.
| Tables        |      Are      |   Cool |
|-------------|:-----------:|-----:|
| col 3 is      | right-aligned | \$1600 |
| col 2 is      |   centered    |   \$12 |
| zebra stripes |   are neat    |    \$1 |
There must be at least 3 dashes separating each header cell. The outer pipes (|) are optional, and you don't need to make the raw Markdown line up prettily. You can also use inline Markdown.
| Markdown | Less      | Pretty     |
|--------|---------|----------|
|_Still_|`renders`|**nicely**|
| 1        | 2         | 3          |

```

Colons can be used to align columns.

[Untitled](https://www.notion.so/b07073e26bed44b0af1ac19b9dca9d6e)

There must be at least 3 dashes separating each header cell. The outer pipes (|) are optional, and you don't need to make the raw Markdown line up prettily. You can also use inline Markdown.

[Untitled](https://www.notion.so/7897ee2ade944377a8483aaa2465b439)

## **[Blockquotes](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#blockquotes)**

```
> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.
Quote break.
> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can_put_ **Markdown** into a blockquote.

```

> Blockquotes are very handy in email to emulate reply text. This line is part of the same quote.
> 

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can put Markdown into a blockquote.
> 

## **[Horizontal Rule](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#horizontal-rule)**

Three or more asterisks...

```
Before.
---
After.

```

Before.

---

After.

### **[Credits](https://meta.stoplight.io/docs/studio/ZG9jOjgz-using-markdown-in-documentation#credits)**

Most of this information was pulled from [Adam Pritchard's Mardkown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). Thank you Adam for putting together this cheatsheet!

## What's Next?

Next you can look into: 

* [**Stoplight Flavoured Markdown**](d.Stoplight-Flavoured-Markdown.md)