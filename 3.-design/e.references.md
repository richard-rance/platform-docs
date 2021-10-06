# References

Often at times, you will find structures in your API projects used across multiple resources. You can avoid duplicity and repetition by reusing these components instead of defining them again. Learn how in this guide. 

## What are References?

Reusing components and reducing repetitions is something we highly recommend at Stoplight. 

And we enable you to do that by leveraging **references** ([$ref](https://swagger.io/docs/specification/using-ref/)) from OAS. References allow splitting of API descriptions across multiple files, for cleaner and more organized code.

![R1.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/20SLsZHuovk)

Using References, you can reuse: 

- Common structures like models, reducing repetition and allowing them to be used for other purposes like [contract testing](https://apisyouwonthate.com/blog/writing-documentation-via-contract-testing).
- Similar parameters or headers across multiple endpoints.
- Examples for request or response bodies.

> **Note:** You can learn more about references and it's an application by visiting our guide: [**Shared Components**](shared-components.md) 

## Working with References

Working with references is very easy. To make use of $ref:

 1. Once you are inside a project, navigate to your desired endpoint. 

 2. Let's say you have to add a request body, to do that click **JSON Request Body**. 

3. As a result, you'd see the option to add **Schema** and an **Example.** 

![R2.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/J78gLnkKUbY)

4. Within the schema section, you would see the type "**object**" mentioned. That is the default schema **type**, change the type to **$ref.** 
5. With **$ref** (references) you can refer to a structure within the project, within a file, or from an external resource. 

![R3.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/yPQSqLFU5qA)

6. Specify the file you want to reference, and the schema for your request body will be updated accordingly.   

7. You can do the same for response body, headers, examples, and other parameters.  

## What's Next?

Making use of references unlocks your path toward shared components and reusing of components. As the next step you can learn how to make use of: 

1. [**Shared Components**](shared-components.md)
2. [**Shared Models**](shared-components.md)