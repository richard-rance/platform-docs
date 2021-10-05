# Request Maker and Code Snippets

Test how your API is turning out in real time, or get developers to their first request in minutes. Learn how in this guide.  

## What are Code Snippets?

Code snippets play an essential role in helping developers use an API. They give a fair idea of how to call an endpoint, reducing the time to first request massively for yourself, co-workers, or for anyone else working with your API. 

On Stoplight these snippets are auto generated, as soon as you are done with design. You can make use of code snippets, throughout the API lifecycle, during design, development, review or whenever you need to. Use code samples to try out an API or plug them into your production ready apps to start using an API. 

## What is the Request Maker?

Stoplight  has a built in HTTP client which we call Request Maker. It appears in a few places throughout our ecosystem, and in Studio you will see it under the "Try it Now" button in Preview.

The request maker is very much like many other HTTP clients out there, but it knows all about your APIs. It knows every endpoint defined in the API description, it knows what headers need are required or optional, what content type you should send, and if the API description has defined servers, it will let you pick from those.

## Working with Code Snippets

 To work with code snippets: 

1. Navigate to your project and select any of the API endpoints from the API sidebar menu on the left.
2. Next open the endpoint and then click the **Preview** button at the top right of the screen. This gives a sneak peak into how your API documentation will look like. 
3. Click **Try it** to open the console section. The console constructs an API request based on your endpoint design. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/39463050-6efa-4537-89df-3bb2b91e4206/Screen_Shot_2021-08-19_at_8.05.48_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/39463050-6efa-4537-89df-3bb2b91e4206/Screen_Shot_2021-08-19_at_8.05.48_PM.png)

1. The code snippets appear as sample requests. While designing endpoints, this gives a fair idea of how end users will experience your API. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9d3cb0f6-7031-45b9-a252-93854e9aa290/Screen_Shot_2021-08-19_at_11.41.45_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9d3cb0f6-7031-45b9-a252-93854e9aa290/Screen_Shot_2021-08-19_at_11.41.45_PM.png)

1. You can fill in sample dat, and click **Send Request** to see if the API is behaving in a way you would want. 

[https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c927256b-6122-4207-b143-0d88f9abcc50/Screen_Recording_2021-08-19_at_8.10.54_PM.mov](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c927256b-6122-4207-b143-0d88f9abcc50/Screen_Recording_2021-08-19_at_8.10.54_PM.mov)

1. By default you will see code snippets in **Shell / cURL** showing up, which is for working on the command line with a very common library called **`curl`**.

Clicking the dropdown on top of snippet will open different languages, most of which support a few different libraries, you can select from any of these. 

**Note:** These code snippets come from the open-source package httpsnippet, so if you'd like to contribute more, first send them a pull request then open an issue on our GitHub repository.

## Languages Supported

## Code Snippets in Documentation

Code snippets appear alongside API references in documentation for each endpoint. Users can view samples, try out sample requests and even copy-paste snippets into their production ready apps to make use of your APIs. Users can also pick different languages and frameworks according to their need. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/14b9ce7d-f9f0-4a09-a5c3-8dacad033110/Screen_Shot_2021-08-19_at_10.08.07_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/14b9ce7d-f9f0-4a09-a5c3-8dacad033110/Screen_Shot_2021-08-19_at_10.08.07_PM.png)

## **Advanced Code Generation**

If you'd like to go further with code generation, consider looking into on of the many top quality code generators listed on [OpenAPI.Tools](https://openapi.tools/).

## What's Next?

You now know how to work with code snippets on Stoplight. Next you can learn how to work with:

1. Mock Servers
2. Validation and Linting