# Specifying Security Requirements

You can specify security requirements for every endpoint in your API. If you do so, you override any global security requirement you may have specified. If you do not specify a security requirement for an endpoint and there are no global security requirements, it means that this operation does not require authentication.


![Specifying Security Requirements](../assets/specifying security requirements 1.mov)


## Adding Security Requirement for an Endpoint

To add a requirement:

1. Navigate to your project and open your desired endpoint. 
2. Open the endpoint and click the **+** (plus) icon that appears next to **Security** section. 

![ssr2.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/sFt6OyGSvS0)


3. From the dropdown that opens, chose **Add operation security.**
4. Next pick the type of your security scheme by clicking the scheme name. 

![ssr3.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/NPuccDsvBiQ)


5. If the selected security scheme uses *oauth2* and you have defined scopes, optionally enter the scopes required for API access in the scopes input field. Note that *all* scopes must be authorized in the flow.

## What's Next?

As the next you can take a look at: 

- **Documenting API Security**
- **Types of Security Schemas**