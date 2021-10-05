# Specifying Global Security

You can specify global security requirements in the **API Overview**, right below the definition of the security schemes. 

The following applies for global security requirements:

- If you define multiple, the API consumer must follow one of them.
- Global security applies to all API operations unless you define a specific security requirement for them.

![Global Security video](../assets/global secutity video gs1.mov)

To add a requirement:

1. Navigate to your project and open the **API Overview** for your API.

![gs2.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/24OclxThQeg)

2. Click the **+** (plus) icon that appears next to *Global Security*.

3. Choose your security scheme in the dropdown menu.

![gs3.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/gVHTtMZK9vA)


4. If the selected security scheme uses ***oauth2*** and you have defined scopes, optionally enter the scopes required for API access in the **scopes input field**. Note that *all* scopes must be authorized in the flow.
    
![gs4.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/dxd1lohYtkQ)

    
## What's Next?
    
Now that you have learned how to specify security schemes and global security, next you can give these guides a look: 

 - **Specifying Security Requirements**
 - **Documenting API Security**