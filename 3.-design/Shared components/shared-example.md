# Shared Examples

Shared Examples can be applied to a response body, or applied to another model so that it will show up anywhere.
Defining an example gives you more power over how that model is displayed in mock servers and documentation tools and gives a fair idea to both API developers and consumers that what goes inside an API request and what comes out.
Examples make your Code Samples and Reference docs even more helpful.

## Adding shared examples

To add a shared example:

1. Open your project  and navigate to the **Models** folder in your API file.
2. From the models folder, select the model you want to add the example for.

![Shared Example](https://stoplight.io/api/v1/projects/cHJqOjI/images/LWFVng7ELc4)

3. Click the Example button with a "+" sign to add a new example.

4. Specify the example values for your schemas, make sure the values you enter give a fair idea of what should go in, or come out of your request.

> Tip: Make sure the data you enter is compatible with your dummy data, which will help users try out your samples from within the console.

5. When done push changes to Git.

**Now every time you reference a model anywhere, the examples would be included with the model by default.**

## What's next?

You now know how to work with shared components on Stoplight. Next you can learn:

- [**Request Maker**](url)
- [**Mock Servers**](url)
- [**Validation and Linting**](url)
