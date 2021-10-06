# **Validation and Linting**

Stoplight lets you know if you are writing invalid YAML, JSON, or Markdown, or if your API description is not in accordance with its recommended convention. Read this guide to find out how. 

## Overview

When multiple people are working on API design, often the design turns out to be incoherent, inconsistent, and full of errors. As your organization expands, quality control becomes a big problem, and enforcing style guides across your teams becomes impossible. This results in lots of errors, fixes, and redundancies, all of that add to the overhead cost. 

Stoplight fixes this problem by linting and validating your API description during the design process. This provides a practical method for enforcing API design rules over multiple APIs, making your APIs consistent before they even exist. 

**Linting** and v**alidation** are executed through a couple of conventions comprising validation rules and style rules. 

### **Validation Rules**

Validation rules signify whether your generic JSON/YAML, API descriptions, etc are technically correct. Failing to comply by validation tule ends up with an error. 

An example of a validation rule would be requiring unique **`operationIds`** for every operation. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c7ea84b8-ecd2-4c2c-95d8-f6f1475661eb/Screen_Shot_2021-08-30_at_4.05.18_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c7ea84b8-ecd2-4c2c-95d8-f6f1475661eb/Screen_Shot_2021-08-30_at_4.05.18_PM.png)

Validation rules are denoted by a red error sign. 

### **Style Rules**

Style rules are more like opinions, they are not about your OpenAPI being valid, they offer suggestions about naming conventions, missing information that would improve the quality of documentation, etc. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9c8b9e21-3293-47f4-875e-9d59509bfdae/Screen_Shot_2021-08-30_at_4.06.16_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9c8b9e21-3293-47f4-875e-9d59509bfdae/Screen_Shot_2021-08-30_at_4.06.16_PM.png)

Style rules are denoted by a yellow warning sign and typically trigger warnings when enabled.

> **Note:** The Style & Validation rule engine is powered by our open-source project **Spectral**, and **custom rulesets** can be created to produce "style guides" for any sort of JSON or YAML data, like OpenAPI or JSON Schema.

## How do Validation and Linting work?

Linting and Validation are enabled by default for the design files you are working on. You can view errors and alerts near the top left side of the page. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6542773c-1972-475b-8fdf-24f4d2e2ebda/Screen_Shot_2021-08-30_at_4.12.43_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6542773c-1972-475b-8fdf-24f4d2e2ebda/Screen_Shot_2021-08-30_at_4.12.43_PM.png)

Clicking the validation tab expands the errors and warnings in detail. You can click on the individual alert to be taken to the exact line where it exists. 

[https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d09c09d9-6807-4682-a290-811746b531c2/Screen_Recording_2021-08-30_at_4.51.12_PM.mov](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d09c09d9-6807-4682-a290-811746b531c2/Screen_Recording_2021-08-30_at_4.51.12_PM.mov)

To learn in detail  how validation and linting works, go through these guides:

1. **Spectral** 
2. **Creating Custom Linting Rules**
3. **Custom Rulesets**