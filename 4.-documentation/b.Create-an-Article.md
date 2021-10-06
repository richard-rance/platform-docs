# Create an Article

An **article** on Stoplight is a page or document that can be added alongside your reference guides to complete your API documentation. 

Articles can include resources like: Getting Started Guides, Tutorials, Use Cases, FAQs, or any artifact that explains how to make use of your API.

>**Note:** For best practices on how to structure your API documentation, visit our guide: [Documenting your APIs](https://meta.stoplight.io/docs/studio/docs/Documentation/01-getting-started.md). 

## Working with Articles

Working with **articles** is very easy. We have a built-in Markdown editor with a **live preview** where you can either edit existing articles or start from scratch. 

![article video](../assets/Article1.mov)


To render articles we use  [Stoplight Flavored Markdown](https://meta.stoplight.io/docs/studio/docs/Documentation/03a-stoplight-flavored-markdown.md#:~:text=Stoplight%20Flavored%20Markdown%20extends%20CommonMark,object%20in%20a%20specific%20way.), our own version of Markdown rendering engine built on top of [CommonMark.](https://commonmark.org/) 

> **Tip:** You're looking at it right now since we've used it to render every doc in this project!  

Apart from the regular markdown syntax, there's a UI formatter right at top of the editor to format your text. You can also include components such as **Code Samples** and **JSON Schemas** at the click of a button.


![Article 2.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/1Ezur1EO1tg)


Stoplight has some conventions around where API files and documentation files should live. All your **articles** are listed under the **Docs** section. 

![Article 3.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/mzdHIm0T0kg)

You can **categorize** articles unde**r tags**. Use **Tags** wisely to organize your documentation. 

![article 4.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/ZdIwTdGIDTs)


# Creating your first article

1. From your **dashboard**, select the **Project** to which you want to add the article to. 
2. On the **Project** page, click the **Edit** button on the left navbar to open Stoplight Studio. 
3. On the studio switch to the **docs** section. This is where all your **articles** are listed. 
4. Click the **+** button near the top of left bar, or the **Article** button in the start section to create an **article.** 

![article 5.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/TbFvRZDfHHE)


5. This will open a modal box. Add in the article **Title** and **Tags.** Click **Create,** when you are done. 

![article 6.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/K6GYCN9WWPM)



6. Once you have specified the **Title** and **Tags,** you will be taken to the markdown editor. Use **Stoplight Flavored Markdown** to create a rich text article.  

![article 7.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/586PeHuHkeM)


As you make additions to an **Article**, you can visualize it live in the **preview** mode. In case you do not want to preview it, you can toggle the preview mode off by clicking the **Preview** button. 

7. There's a UI component on top of the editor, use the component to format your text if you are not comfortable with Markdown. 

![Article 2.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/6aFfUthmPvc)


8. With the UI component, you can also add **Code Snippets** or **JSON Schemas** to your documentation. 

## Code Snippets:

Code Snippets in Stoplight come as part of the **HTTP request maker.** The **[Request Maker](../3.-design/g.requestmaker.md)** makes your articles interactive. 

Code snippets give a decent idea of how your API is going to look in real-time, and how to consume it. With the **Request Maker**, users can try out your API on spot, without having to write code for themselves. 

![article 8.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/zdqzxf2F09w)


>**Note:** To learn more about how to make use of the **Request Maker**, visit our guide: [Request Maker](../3.-design/g.requestmaker.md)

### **JSON Schemas:**

With JSON Schemas you can show in an **article** how **data structures** in your API will look like.  

![article 9.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/pJjK1dFZpCY)


9.  Within an article, you can also place images. Learn how to work with images in our detailed guide: **[Adding Images](e.Images.md)** 

10. Once you are done, commit and push the **Article** to your repo. 



**That's it. You just created your first article on Stoplight. ✍️**

## **What's Next?**

Now that you know how to create articles find out what next steps you can follow: 

1. **[Share Documentation](h.Creating-external-Documentation.md)** 
2. **[Create a Home Screen](Customizing-Docs/a.homescreen.md)** 
