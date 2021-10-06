# Mock Servers

Having a mock server can be really handy throughout the design phase of an API for making sure API descriptions contain the right sort of information.

## What are Mock Servers?

Stoplight offers free, automatically updated HTTP mock servers for every API published in your workspace. These mock servers simulates real APIs, by providing endpoints and validation rules described in your API description document.

> **Note:** Our hosted mock servers are powered by our open-source mock server Prism, so if you are familiar with this tool then you'll be familiar with hosted mocking.

Within "Try it Now" you can talk to any server, but if you want to talk to the mock server open up the "Mocking" tab and enable it. Now any requests will be sent to the mock server, so you can get a feel for how this API is going to respond.

## **Interacting with Mock Servers**

In the same way that documentation is updated on publish (or on push), mock servers are updated when pushing to the default branch. 

To talk to the HTTP mock servers, there's a few options.

### 1. Explorer and Docs

The **Try it** section in Docs and Explorer has hosted mocking built- in. You just need to enable mocking from the Mocking tab, and you're good to go.

Enabling the mock server on **Try It** section will send requests to the mock server, so you can get a feel for how the API will respond.

### 2. Any HTTP Client

If that does not seems useful, you can just take the **Mock Server URL** and compose the whole URL yourself.

![Mockserver video](../assets/MockServer M1 .mov)



Consider the mock server to be a special server, just one that's not mentioned in your API description. So if you had an OpenAPI description with the following servers...

```json
servers:
  - description: Production
    url: "https://api.example.com"
  - description: Staging
    url: "https://api.staging.example.com"
paths:
  /hello:
    get: 
      # ...

```

You could swap out that URL for your Hosted Prism URL:

[https://workspacename.stoplight.io/mocks/workspacename/todos](https://workspacename.stoplight.io/mocks/workspacename/todos)

The actual contents of the responses depends on the examples in the API Description, and if the request prefers static or dynamic mode, and if you requested specific status codes to come back.

To use mock server on the **API Explorer**: 

![M2.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/EROShFbeJe0)


1. Click Explore on the left nav-bar of your workspace. 
2. Navigate to your endpoint, and click it. 
3. In the Try it section, click mocking and then click enable. 
4. Your URL will now be replaced with the mock server URL. 
5. Click **Send request** to try it out. 

To use mock server on **Docs**: 

![M3.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/lAVqdUTUJKM)


1. Navigate to your project on your workspace. 
2. Click on the Project name to open Docs. 
3. Select the endpoint you want to mock. 
4. In the **Try it** section, scroll down to **mocking**. 
5. Click **enabled** on the dropdown that opens. 
6. Your URL will now be replaced with the mock server URL. 
7. Click **Send request** to try it out. 

> Note: For the open source mock server CLI visit our guide: **PRISM CLI**

## What's Next?

Mock servers offer great utility in testing out an API while you design. Once you know how to make use of them, you can take a look at: 

- **Design Review Process**
- **API Security**