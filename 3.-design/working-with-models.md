# Working with Models

Stoplight's schema editor allows you to easily design and model data structures used by your API. In this guide learn how you can make use of the editor to define your models. 

## What are Models?

Models are the schemas that go in your API's request or response bodies. Models can be of either:

1. **Primitive type**: String, integer, array, boolean
2. **Complex type** (object): That you can define yourself.

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/31a94314-0927-45b4-a90e-c07eb98415a8/Screen_Shot_2021-03-16_at_5.46.47_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/31a94314-0927-45b4-a90e-c07eb98415a8/Screen_Shot_2021-03-16_at_5.46.47_PM.png)

> **Tip:** Learn more about modeling your schemas, you can visit the official OpenAPI documentation here: [https://swagger.io/docs/specification/data-models/](https://swagger.io/docs/specification/data-models/)

Defining a model can be hard work, but on Stoplight Studio you can easily do that in two different ways: 

- **JSON Schema Editor:**  UI form-based ****editor to create data structures in an easy-to-use, graphical format.
- **Raw Schema** **Editor:** Paste or type raw JSON to generate a model.

While each method can be used individually, you will most likely find yourself using a combination of both methods while drafting API endpoints, models, and responses.

## **Using the Schema Editor**

Stoplight Studio's UI schema editor makes modeling very simple and easy. You can find the JSON Schema editor within any model or endpoint while **[Form View](https://meta.stoplight.io/docs/studio/docs/ui-overview.md)** is selected. To start making use of the editor:

1. Open your API file in Stoplight Studio and navigate to your endpoint. 
2. Once the endpoint is open, scroll down and click on **JSON Request Body** or **Response.** This will open the **scheme editors** for them. 
    
    
    [https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d378d87f-c424-410b-8b40-b9cb671a2ca1/Screen_Recording_2021-03-16_at_6.02.49_PM.mov](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d378d87f-c424-410b-8b40-b9cb671a2ca1/Screen_Recording_2021-03-16_at_6.02.49_PM.mov)
    

3.  Click the **+** (plus) icon next to the root **object** to start adding fields to the data structure. The plus icon can also be used on nested objects to create a hierarchy of nested data structures. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9e61f85e-0a04-45e4-b130-7921d4ad01f7/Screen_Shot_2021-03-16_at_6.14.40_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9e61f85e-0a04-45e4-b130-7921d4ad01f7/Screen_Shot_2021-03-16_at_6.14.40_PM.png)

For the new field, specify a: 

1. **Name:** Names can be composed of any alphanumeric characters, but can only be specified once. 

**Warning:** You will receive an error if you try to re-use field names multiple times on the same level (though they can be re-used on nested objects)

 2.  **Type:**  The default type for a newly-created field is '**string**', however other types include:

- objects (for nesting objects)
- arrays
- numbers
- integers
- booleans
- nulls
- [references](https://meta.stoplight.io/docs/studio/docs/Design-and-Modeling/07-using-references.md) (a.k.a. shared components)

Field types can also include *Combination Types*, which include 'allOf', 'oneOf', and 'anyOf'. These special types allow for object inheritance from other data structures and models.

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/41d530cf-1b2e-472e-9883-dd55cc565133/Screen_Shot_2021-03-16_at_8.41.50_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/41d530cf-1b2e-472e-9883-dd55cc565133/Screen_Shot_2021-03-16_at_8.41.50_PM.png)

 3. **Description:** Include a small description to explain the field. The description goes in your public documentation and should give a fair idea of what the consumer should expect. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a2db9db9-ed78-4182-b379-ae6d9a681974/Screen_Shot_2021-03-16_at_8.43.26_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a2db9db9-ed78-4182-b379-ae6d9a681974/Screen_Shot_2021-03-16_at_8.43.26_PM.png)

4. **Mark Required:** Specify field as required, which ensures that the field is present in all requests (and an error is thrown otherwise).

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9ef4f3c6-2851-42b4-be6d-d51b5c9759f2/Screen_Shot_2021-03-16_at_9.24.38_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9ef4f3c6-2851-42b4-be6d-d51b5c9759f2/Screen_Shot_2021-03-16_at_9.24.38_PM.png)

5. **Default Value:** Specify a default value for a field, for instance, if the field is boolean, the default value can be **true** or **false**.

6: **Example:**  Example values again help with documentation, and helps builds better code samples. Make sure example values are valid according to the field type. 

7. **Enumerations:** *Enums* for short, allow you to restrict the contents of the field to be specific values. For example, if you are creating a 'color' field of type string, you may want to restrict the strings used in that field to specific colors (red, blue, green, etc).

8. **Format:** Describe the specific format of a field, like a date, time, IP address, URI, email, etc.

9. **Mark Deprecated:** You can mark the field deprecated if it has been. 

10. **Pattern:** Specify a pattern of acceptable values, these change with field type. 

11. **Mark Read/Write:** Fields marked read-only can only be retrieved and not changed. 

**Note:** When creating a **[shared model](https://www.notion.so/Shared-Models-203f291067d34b38b7380a379e2139fe)**, you can also specify a model **Name** and **Description.**

## **Editing the Raw JSON Schema**

If UI editor is not something you are comfortable with, you can make use of the raw **JSON** editor to either copy-paste JSON representation of your schemas or start from scratch. 

To start doing that:

[https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a4d4a975-7078-4ae8-9131-2b106dd45da0/Screen_Recording_2021-06-29_at_8.53.55_PM.mov](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a4d4a975-7078-4ae8-9131-2b106dd45da0/Screen_Recording_2021-06-29_at_8.53.55_PM.mov)

1. Open your API file in Stoplight Studio and navigate to your endpoint or model. 
2. Near the top left of the editor, click the **</Code>** button to toggle to raw JSON editor. 
3. You can toggle back using the form button. 
4. Alternatively, you can also click **Generate from JSON button on** schema editor to use work with raw JSON instead of UI. 

> **Tip:** When modeling endpoints, you can use [our built-in HTTP client](https://meta.stoplight.io/docs/studio/docs/Design-and-Modeling/05-request-maker.md) to hit either a real API (a development server, production, etc) or a [mock server](https://meta.stoplight.io/docs/studio/docs/Design-and-Modeling/06-mock-servers.md).

## What's Next?

As the next step you can look into: 

- **[Shared Components](url)**
- [**Request Maker**](url)
- **Mock Server**