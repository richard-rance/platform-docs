# **Shared Parameters**

**Parameters** are the variable part of an HTTP request. They are the options that can be passed along with an endpoint to influence the response. Describing a HTTP request involves talking about the URL, method, body, all of which are covered elsewhere, but everything else is a parameter.

There can be multiple types of parameters that can go in a request, these include: 

- **path** - Dynamic values in the path part of the URL, e.g.: `/people/{id}`.
- **query** - Dynamic values in the query string part of the URL, e.g.: `/planets?name=Endor`.
- **header** - Custom headers that are expected as part of the request.
- **cookie** - Used to pass a specific cookie value to the API.

According to OpenAPI conventions, each parameter can have **attributes** and **validations** to describe things like **data types**, **default values and examples.** Parameters can also be **restricted** to a specific set of values (enum), or marked as **deprecated** to signal to API consumers that they should no longer be used. On Stoplight's intuitive editor, you can easily specify all of these details. 

## Adding a new shared parameter

To add a new parameter: 

1. Navigate to and open your project. 
2. Scroll to the bottom of your API file, to the **Parameters** folder. 
3. Right-click, on the "Parameter" section heading, select the **type** of parameter and specify a **name.** And then specify parameter details. 

![Create Parameter](../assets/SP2.mov)


4. For a parameter, you can specify: 

![Specify Parameter](https://stoplight.io/api/v1/projects/cHJqOjI/images/cOvlveEVP4s)

Name, field type, description, and properties including: format, default value, min length or  max length, pattern for a list of accepted values, if it's deprecated (or not), or if empty values are allowed. 

5. You can delete a parameter by simply clicking the delete button above. 

![Delete Shared Parameter.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/cdhfJPGfNZ8)


## Using Shared Parameter on Stoplight

To use a **shared parameter**: 

1. Navigate to an **API endpoint** in your project and click on either query or path, or header parameter button.  

2. For any of these **parameters**, click the **chain link icon** button (reference button), this will let you reference the shared parameter. 

![Watch the video](../assets/SM.mov)

Once the parameter has been referenced, any updates to the shared parameter will automatically be propagated to every endpoint using that parameter. Like other references in Stoplight, shared parameters can also be shared across files, projects, and other external sources.

## **Shared Parameters Example**

Let's say you are creating an API to serve thousands of cooking recipes. When dealing with large volumes of data, you typically want to avoid sending *all* data in a request. To help avoid sending more data than is necessary, most applications implement a "paging" feature that allows clients to retrieve a small portion of results (i.e. a single page).

There are multiple ways to approach a paging feature. For this example, we want to add two query string parameters to every request:

- `limit` - The number of results to return when viewing a page. For example, setting `limit` to `20` means that, at most, 20 results will be returned in the request.
- `offset` - The number of results to skip before returning results. For example, setting an `offset` of `20` means that the API will discard the first 20 results.

By using the two parameters above, a client can efficiently "page" through results, only returning items that are within the requested bounds. To demonstrate, let's use the parameters to display the first page of our recipe results:

```
GET /recipes?limit=20&offset=0
```

Since the `offset` is set to `0`, the API will not discard any results. Paired with a `limit` of `20`, we will only see the first 20 results (1 through 20).

To view the second page of recipes, we would use:

```
GET /recipes?limit=20&offset=20
```

By setting an `offset` of `20`, the API will discard the first 20 results. Paired again with a `limit` of `20`, we will see the second page of results (21 through 40).

## What's Next?

- **Shared Responses**
- [**Shared Models**](Shared-Models.md)
- **Shared Examples**