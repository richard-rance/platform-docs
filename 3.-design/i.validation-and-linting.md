# **Validation and Linting**

Stoplight lets you know if you are writing invalid YAML, JSON, or Markdown, or if your API description is not in accordance with the recommended convention. Read this guide to find out how to best make use of this. 

## Overview

When multiple people are working on API design, often the design turns out to be incoherent, inconsistent, and full of errors. As your organization expands, quality control becomes a big problem, and enforcing style guides across your teams becomes impossible. This results in lots of errors, fixes, and redundancies, all of that add to the overhead cost. 

Stoplight fixes this problem by **linting** and **validating** your API description during the design process. This provides a practical method for enforcing API design rules over multiple APIs, making your APIs consistent before they even exist. 

**Linting** and v**alidation** are executed through a couple of conventions comprising **validation rules** and **style rules**. 

### **Validation Rules**

Validation rules signify whether your generic JSON/YAML, API descriptions, etc are technically correct. Failing to comply by validation tule ends up with an error. 

An example of a validation rule would be requiring a unique **`operationIds`** for every operation. 

![vl1.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/FuAoB3DFs3I)


Validation rules are denoted by a **red error sign**. 

### **Style Rules**

Style rules are more like opinions, they are not about your OpenAPI being valid, they offer suggestions about naming conventions, missing information that would improve the quality of documentation, etc. 

![vl2.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/DwaZfJvTY54)


Style rules are denoted by a **yellow warning sign** and typically trigger warnings when enabled.

> **Note:** The Style & Validation rule engine is powered by our open-source project **Spectral**, and **Custom rulesets** can be created to produce "style guides" for any sort of JSON or YAML data,like OpenAPI or JSON Schema.

## How do Validation and Linting work?

Linting and Validation are enabled by default for the design files you are working on. You can view errors and alerts near the top left side of the page. 

![vl3.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/QQurTPsW7mg)


Clicking the validation tab expands the errors and warnings in detail. You can click on the individual alert to be taken to the exact line where it exists. 

![vl video](../assets/VLvideo.mov)

To learn in detail  how validation and linting works, go through these guides:

1. **Spectral** 
2. **Creating Custom Linting Rules**
3. **Custom Rulesets**