# Links

You can add links to your articles for better navigation. Your links can point to both, files within your projects, and external resources. Learn how to work with them in this guide. 

## What are links?

Links in your articles point users to content on the same page, to other pages in your projects, or to external sites and URLs.  

Stoplight Flavored Markdown (SMD) treats links the same way as regular markdown and uses the similar syntax. 

This is how links will look on your pages once you include them in your files. 

![links1.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/tWAnv8UF3zM)


The three most common form of links include: 

1. **Article to article:** to point to another article within your project. 
2. **Anchor link:** to jump within a specific article
3. **External link:** To point to a web resource outside your project. 

> **Tip:** Instead of using "click here" for your display text, make use of actual titles of the resources you are linking to. 

## Using links in documentation

Adding links to your documentation is very easy. There are three ways you can do it.  

## 1. Article to article link:

Create hyperlinks to other articles within your projects to create additional navigation. To add links between articles: 

1. Open your project in **Studio,** and select the **file** you wish to modify. 
2. Use this syntax to construct your link

`[Display Text](Hyperlink URL/File Location)`

In the `Display Text` enter the **article** name, and link the `(Hyperlink URL/File Location)` section. 

**Example:**

 `[API Design Quickstart Guide](../Design-and-Modeling/01-getting-started.md)`

- To link an article from the same folder, you can use:

       `[Display text](article-name.md)`

- To link an article in the parent folder:
    
    `[Display text](../article-name.md)`
    
- To link an article in a subfolder:
    
    `[Display text](folder/article-name.md)`
    

## 2. Anchor links:

Anchor links help readers jump within articles to a specific section, so they don't have to scroll all the way up or down. Consider it as an interactive table of contents. 

For instance, this tag will take you to top of the page: [**Using Links**](https://meta.stoplight.io/docs/platform/branches/DocsV4/ZG9jOjIzMzk0NjA2-links#what-are-links)

To add **anchor links** in your articles:

1. Open the file you wish to modify 
2. Add in the following syntax:  
- To direct reader to section on same page:

      `[Display text](#anchor-text)`

- To direct reader to a section on different page:

     `[Display text](filename.md#anchor-text)`

> **Note:**  Anchor text must always be lowercase and not contain spaces.

## 3. External links:

You can also link readers to external resources that sit outside your projects, for instance your blog, FAQ section, or your pricing page. 

To add **external links** in your articles:

1. Open the file you wish to modify 
2. Add in the following syntax:  

`[Display text](URL)`

**Example:** 

`[Display text](https://stoplight.io/)`

**You now know how to add links in your articles, and can create richer documentation that ever!**  📎



## What's next?

Since you are now we aware of how to create your documentation articles, let's head over to 

- **[Redirects](g.redirects.md)**
- **[Sharing documentation](h.Creating-external-Documentation.md)**