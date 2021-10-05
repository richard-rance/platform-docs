# Shared Components
When using Stoplight, or OpenAPI in general, there are various resources that can be either defined within an endpoint or reused between multiple endpoints.
Reusing components makes processes more agile and efficient, and is something we highly recommend at Stoplight. In this guide learn how can you ensure reusability of components while designing your APIs.

## What are Shared Components?

Often within API projects, there are resources such as parameters, schemas, or responses that can go in one or multiple endpoints, but as you chalk out each individual request, you have to specify these components every single time.
Each of these components can have several underlying details, and typing them out over and over again, can hurt your team's efficiency, and increases the chances of errors.

To avoid this duplication, you can define these components once and the next time you need them, instead of having to enter them again, just put a reference.

These components are called shared components. In Stoplight they come in several forms:

* **Parameters** - Parts of the request: query string parameters, path parameters, headers, and cookies.
* **Responses** - Common responses like page not found, validation errors, etc.
* **Models** - Also known as "Schemas", these are the most common shared component. They describe the actual shape of the data for JSON requests and responses.
* **Examples** - Show how a request or response body might look. These can be generated from schemas automatically, but can also be made manually created for more complex scenarios.

## Using Shared Components
Making use of **shared components** is very easy.
Once you are inside your project navigate to your endpoint and look for the reference button, alongside your desired component.

Click the reference button, this will open the potential list of options you have available for that component.
Select your desired option and you are done.

## Adding a new Shared Components
To create a shared component:

1. Scroll to the end of your API file on the Studio, and right-click the component name.
2. Specify component details, and click save, as an example, we are adding a query parameter in the video below.

![Shared component](../assets/SP2.mov)


Once done push changes to Git. 

## What's next?

You now understand the basics of using Shared Components. To learn how to make use of components in detail, visit our guides:

- [**Shared Parameters**](shared-parameters.md)
- [**Shared Models**](shared-models.md)
- [**Shared Examples**](shared-example.md)

