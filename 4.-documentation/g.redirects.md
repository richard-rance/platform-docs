# Redirects
Want to move your documentation pages without breaking old links? You can manually configure redirect rules for paths on your Workspace's custom domain.

![Red0.jpeg](https://stoplight.io/api/v1/projects/cHJqOjI/images/Tvv4Pc9KvVI)


## What are Redirects?
When you move your documentation to new pages or addresses, you will often find your customers landing on the old pages. To make sure it does not spoil their experience, you can manually configure redirects on Stoplight, so customers are always routed to the correct page.

>**Note**: This feature is available on the **[Stoplight Starter plan](https://stoplight.io/pricing/)**, and above.

## How does it work ?

Before you get started, you need to snure your workspace is hosted on a Custom Domain. 

>**Note:** To find out how to configure custom domains visits our guide: **[Custom Domains](CustomizingDocs/c.custom-domain.md)** 

When someone navigates to a path matching one of your redirect rules, they will automatically be redirected to the new path. To get strated: 

1. Navigate to your Stoplight Workspace **settings** and scroll down to  the **Custom Domains** section. 

![Red1.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/iOZjvqInYfg)


2. Next click Redirects in the Customs Domain section. This will open a text editor, enter your redirect rule. 
3. There can be one or multiple rules. Each redirect rule must be listed on a separate line, with the original path followed by a space then the new path. 

![Red2.jpeg](https://stoplight.io/api/v1/projects/cHJqOjI/images/T9W77pwHct8)


4. Lines beginning with # will be ignored. You can use the # sign for comments. 
5. There are multiple types of redirect rules that you can configure. 

6. Once you have entered a new rule, click **Save.** 

## Types of Redirect Rules

### Redirect to new path:

To move a page to a new location, you can use a rule like this. The old address is replaced with the new address. 

**Example:** 

```json
# Old path         New path
/old/introduction /docs/my-project/introduction
```

### Redirect all subpaths to a new path:

To remove several pages and replace them with a single page, you would need this rule. All the pages on that path will then point towards your new page. 

**Example:** 

```json
# Old paths     New path
/old/welcome/* /docs/my-project/introduction
```

Then when someone navigates to a subpath of /old/welcome/ such as [https://your-domain.com/old/welcome/overview](https://your-domain.com/old/welcome/overview), they will automatically be redirected to [https://your-domain.com/docs/my-project/introduction](https://your-domain.com/docs/my-project/introduction).

### Redirect all subpaths to a matching subpath:

To move several articles from one location to another, you can redirect users to a new subpath, but the same destination links. 

**Example:** 

```json
# Old paths    New paths

/old/guides/* /docs/my-project/*
```

With this, when someone navigates to a subpath of **`/old/guides/`**, such as **`https://your-domain.com/old/guides/quickstart`**, they will automatically be redirected to a destination with the same subpath: **`https://your-domain.com/docs/my-project/quickstart`**.

## What's Next?

Now that you know how to confifure redirects, you can learn how to: 

- **[Publish Documentation](4.-documentation/h.Creating-external-Documentation.md)**
- **[Configure Custom Domain](CustomizingDocs/c.custom-domain.md)**