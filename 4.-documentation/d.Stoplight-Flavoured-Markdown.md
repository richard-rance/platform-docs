# **Stoplight Flavored Markdown (SMD)**

At Stoplight we have built our own flavour of markdown building on top of CommonMark project.  Stoplight Flavored Markdown (**SMD**) extends Github style fo documentation with inline comment annotations. Learn in this article how to use the various new components we introduced while creating docs on Stoplight. 

## **[Overview](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#overview)**

Stoplight Flavored Markdown can be used to enhance existing Markdown documentation with necessary documentation components like code blocks, images, diagrams e.t.c.

### **[Components](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#components)**

- [Callouts](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#callouts)
- [Task Lists](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#task-lists)
- [Code Blocks](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#code-blocks)
- [Code Groups](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#code-groups)
- [Images](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#images)
- [Graphs and Diagrams](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#graphs-and-diagrams)
- [JSON Schema](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#json-schema)
- [Tabs](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#tabs)
- [HTML Support](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#html)
- [Embeds](https://meta.stoplight.io/docs/studio/ZG9jOjg0-stoplight-flavored-markdown-smd#embeds)

### **The Two Laws**

1. SMD is human readable. A human with a simple text editor can easily read and write SMD.
2. SMD degrades gracefully. SMD documents rendered on **`github.com`** should be clean and readable.

### **The Approach**

1. Stoplight Flavored Markdown extends GitHub Flavored Markdown with inline comment annotations.
2. The value inside of the annotations is a YAML object, and the annotation affects the Markdown block that directly follows it in the document.

By leveraging comments to store annotations, Stoplight Flavored Markdown degrades gracefully to any other Markdown renderer (GitHub, for example).

## **Callouts**

A callout is an MD blockquote with an optional annotation that indicates intent.

### **Danger**

> Danger Will Robinson!Here is my danger callout!
> 

```
Copy this code to try it out!
<!-- theme: danger -->
> #### Danger Will Robinson!
>
> Here is my danger callout!

```

### **Warning**

> Watch Out!Here is my warning callout!
> 

```
Copy this code to try it out!
<!-- theme: warning -->
> #### Watch Out!
>
> Here is my warning callout!

```

### **Success**

> Mission Accomplished!Here is my success callout!
> 

```
Copy this code to try it out!
<!-- theme: success -->
> #### Mission Accomplished!
>
> Here is my success callout!

```

### **Info**

> A thing to knowHere is my info callout
> 

```
Copy this code to try it out!
<!-- theme: info -->
> #### A thing to know
>
> Here is my info callout

```

## **Task Lists**

- [ ]  one
- [x]  two
- [ ]  three

```
Copy this code to try it out!
- [ ] one
- [x] two
- [ ] three

```

## **Code Blocks**

An SMD code block is an MD code fence with an optional annotation to tweak the presentation of the code block.

**Supported annotations**:

- **title**: Title for the code snippet
- **lineNumbers**: True/False to toggle line number visibility

### **Markdown Annotations**

**javascript**

**example**

**`My code snippet passed via md annotations**1function fibonacci(num) {2  var a = 1,3    b = 0,4    temp;56  while (num >= 0) {7    temp = a;8    a = a + b;9    b = temp;10    num--;11  }1213  return b;14}`

### **Meta Tag Annotations**

You can also pass the annotations via the code block meta tag.

**json**

**example**

**`Passed via meta tag**1{2  "foo": "bar"3}`

## **Code Groups**

If you write multiple code blocks with no other content between them they will be grouped into a tabbed code group. This functionality is helpful for a variety of use cases, such as displaying code samples in a variety of languages.

> Note that code groups cannot be nested in other elements like tabs.
> 

**js**

**ruby**

**php**

**`Code groups work with titles and other annotations!**1// Install via npm2npm install --save my-library`

## **Images**

Use annotations to frame up product images.

### **Default**

The default setting adds an outline and click to zoom for images.

![https://stoplight.io/images/home/logo-blue-black.png](https://stoplight.io/images/home/logo-blue-black.png)

```
Try it out!
![Stoplight Logo](https://stoplight.io/images/home/logo-blue-black.png)

```

### **Center Focus**

Make screenshots pop out with a center focus and a default background image.

![https://i.imgur.com/YCb6MWI.png](https://i.imgur.com/YCb6MWI.png)

```
Try it out!
<!-- focus: center -->
![Dev portal settings](https://i.imgur.com/YCb6MWI.png)

```

### **Add a Caption**

Add an optional caption to explain the screenshot further.

**Can add an optional caption**

![https://i.imgur.com/ueOOL8X.png](https://i.imgur.com/ueOOL8X.png)

```
Try it out!
<!-- focus: top -->
![Studio project share](https://i.imgur.com/ueOOL8X.png 'Can add an optional caption')

```

### **Try a Different BG Color**

![https://i.imgur.com/ueOOL8X.png](https://i.imgur.com/ueOOL8X.png)

```
Try it out!
<!--
focus: top
bg: primary
-->
![Studio project share](https://i.imgur.com/ueOOL8X.png 'Can add an optional caption')

```

### **Use a hex BG Color**

![https://i.imgur.com/ueOOL8X.png](https://i.imgur.com/ueOOL8X.png)

```
Try it out!
<!--
focus: top
bg: "#f78ae0"
-->
![Studio project share](https://i.imgur.com/ueOOL8X.png)

```

### **Good Old Plain Images**

![https://i.imgur.com/ueOOL8X.png](https://i.imgur.com/ueOOL8X.png)

```
Try it out!
<!--
focus: false
-->

```

## **Graphs and Diagrams**

You can add graphs and diagrams in your Markdown via the **`mermaid`** code block language tag. Here are some examples:

> Note that diagrams cannot be nested in other elements like tabs or code groups.
> 

### **Flowchart**

**mermaid**

**example**

### **Sequence**

**mermaid**

**example**

AliceJohnBobHello John, how are you?1Fight against hypochondria2loop[Healthcheck]Rational thoughts!Great!3How about you?4Jolly good!5AliceJohnBob

### **Journey**

**mermaid**

**example**

CatMeMy working day

## **JSON Schema**

The SMD JSON schema block is an MD code block with an additional **`json_schema`** language tag. The contents of the code fence should be the JSON schema object to be rendered. The primary language tag can be **`YAML`**, **`YML`**, or **`JSON`**.

User

**id**

stringrequired

**name**

stringrequired

The user's full name.

**age**

number

>= 0<= 150

Try it out with the example below:

```
Try it out!
```json json_schema
{
  "title": "User",
  "type": "object",
  "properties": {
    "id": {
      "type": "string"
    },
    "name": {
      "type": "string",
      "description": "The user's full name."
    },
    "age": {
      "type": "number",
      "minimum": 0,
      "maximum": 150
    }
  },
  "required": ["id", "name"]
}

```

## **Tabs**

An SMD tab container is a **`tab`** annotation, followed by the tab content, and closed by a final **`tab-end`** annotation.

> Tab containers cannot be nested.
> 

**My First Tab**

**My Second Tab**

The contents of tab 1.

```
Try it out!
<!--
type: tab
title: My First Tab
-->
The contents of tab 1.
<!--
type: tab
title: My Second Tab
-->
The contents of tab 2.
<!-- type: tab-end -->

```

## **HTML**

Most basic HTML is supported. **However, we highly recommend using the Markdown equivalent whenever possible.**

[Untitled](https://www.notion.so/08094ed3074a45c6abe85fe9af2f056f)

---

## **Embeds**

> This hasn't been implemented yet. Vote for this feature!
> 

This is a YouTube video:

[https://www.youtube.com/watch?v=aoLhACqJCUg](https://www.youtube.com/watch?v=aoLhACqJCUg)

This is a photo:

[https://www.flickr.com/photos/pedrocaetano/27432477888](https://www.flickr.com/photos/pedrocaetano/27432477888)

This is another photo:

[http://www.23hq.com/mprove/photo/66422006](http://www.23hq.com/mprove/photo/66422006)