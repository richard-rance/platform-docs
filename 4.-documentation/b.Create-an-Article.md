# Create an Article

An **article** on Stoplight is a page or document that can be added alongside your reference guides to complete your API documentation. 

Articles can include resources like: Getting Started Guides, Tutorials, Use Cases, FAQs, or any artifact that explains how to make use of your API.

>**Note:** For best practices on how to structure your API documentation, visit our guide: [Documenting your APIs](https://meta.stoplight.io/docs/studio/docs/Documentation/01-getting-started.md). 

## Working with Articles

Working with **articles** is very easy. We have a built-in Markdown editor with a **live preview** where you can either edit existing articles or start from scratch. 

[https://s3-us-west-2.amazonaws.com/secure.notion-static.com/11ca7ccc-d661-4b4c-8a64-23e93cb8bcaf/Screen_Recording_2021-02-19_at_8.00.50_PM.mov](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/11ca7ccc-d661-4b4c-8a64-23e93cb8bcaf/Screen_Recording_2021-02-19_at_8.00.50_PM.mov)

To render articles we use  [Stoplight Flavored Markdown](https://meta.stoplight.io/docs/studio/docs/Documentation/03a-stoplight-flavored-markdown.md#:~:text=Stoplight%20Flavored%20Markdown%20extends%20CommonMark,object%20in%20a%20specific%20way.), our own version of Markdown rendering engine built on top of [CommonMark.](https://commonmark.org/) 

> **Tip:** You're looking at it right now since we've used it to render every doc in this project!  

Apart from the regular markdown syntax, there's a UI formatter right at top of the editor to format your text. You can also include components such as **Code Samples** and **JSON Schemas** at the click of a button.

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9411cdb2-3534-4bc9-90eb-2dd50d5d6b6e/Screen_Shot_2021-02-12_at_12.42.22_AM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9411cdb2-3534-4bc9-90eb-2dd50d5d6b6e/Screen_Shot_2021-02-12_at_12.42.22_AM.png)

Stoplight has some conventions around where API files and documentation files should live. All your **articles** are listed under the **Docs** section. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c953cda5-d3cd-4d74-8800-f2adb166f0be/Screen_Shot_2021-02-19_at_7.13.25_PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c953cda5-d3cd-4d74-8800-f2adb166f0be/Screen_Shot_2021-02-19_at_7.13.25_PM.png)

You can **categorize** articles unde**r tags**. Use **Tags** wisely to organize your documentation. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/75375237-d02b-4373-a756-71013c10dfa3/Screen_Shot_2021-02-12_at_12.38.28_AM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/75375237-d02b-4373-a756-71013c10dfa3/Screen_Shot_2021-02-12_at_12.38.28_AM.png)

# C**reating your first article**

1. From your **dashboard**, select the **Project** to which you want to add the article to. 
2. On the **Project** page, click the **Edit** button on the left navbar to open Stoplight Studio. 
3. On the studio switch to the **docs** section. This is where all your **articles** are listed. 
4. Click the **+** button near the top of left bar, or the **Article** button in the start section to create an **article.** 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b268e7c4-0201-4ce1-87fa-d99a3cd9828e/Screen_Shot_2021-02-12_at_12.25.28_AM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b268e7c4-0201-4ce1-87fa-d99a3cd9828e/Screen_Shot_2021-02-12_at_12.25.28_AM.png)

4. This will open a modal box. Add in the article **Title** and **Tags.** Click **Create,** when you are done. **** 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/da99c1b3-72dd-4970-9015-05e3275c3a0f/Screen_Shot_2021-02-11_at_1.32.41_AM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/da99c1b3-72dd-4970-9015-05e3275c3a0f/Screen_Shot_2021-02-11_at_1.32.41_AM.png)

7. Once you have specified the **Title** and **Tags,** you will be taken to the markdown editor. Use **Stoplight Flavored Markdown** to create a rich text article.  

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1c020bb8-c0b9-450b-8c8e-06e7087956c5/Screen_Shot_2021-02-11_at_1.32.57_AM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1c020bb8-c0b9-450b-8c8e-06e7087956c5/Screen_Shot_2021-02-11_at_1.32.57_AM.png)

As you make additions to an **Article**, you can visualize it live in the **preview** mode. In case you do 

not want to preview it, you can toggle the preview mode off by clicking the **Preview** button. 

8. There's a UI component on top of the editor, use the component to format your text if you are not comfortable with Markdown. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9411cdb2-3534-4bc9-90eb-2dd50d5d6b6e/Screen_Shot_2021-02-12_at_12.42.22_AM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9411cdb2-3534-4bc9-90eb-2dd50d5d6b6e/Screen_Shot_2021-02-12_at_12.42.22_AM.png)

9. With the UI component, you can also add **Code Snippets** or **JSON Schemas** to your documentation. 

### Code Snippets:

Code Snippets in Stoplight come as part of the **HTTP request maker.** The **Request Maker** makes your articles interactive. 

Code snippets give a decent idea of how your API is going to look in real-time, and how to consume it. With the **Request Maker**, users can try out your API on spot, without having to write code for themselves. 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c4111f47-d6e9-4df3-9372-b310e15130d7/Screen_Shot_2021-02-12_at_2.11.45_AM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c4111f47-d6e9-4df3-9372-b310e15130d7/Screen_Shot_2021-02-12_at_2.11.45_AM.png)

>**Note:** To learn more about how to make use of the **Request Maker**, visit our guide: [Request Maker](../3.-design/g.requestmaker.md)

### **JSON Schemas:**

With JSON Schemas you can show in an **article** how **data structures** in your API will look like.  

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/54a8a965-1e32-4c00-b55e-e0384f37037f/Screen_Shot_2021-02-12_at_2.28.24_AM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/54a8a965-1e32-4c00-b55e-e0384f37037f/Screen_Shot_2021-02-12_at_2.28.24_AM.png)

10.  Within an article, you can also place images. Learn how to work with images in our detailed guide: **Adding Images** 

11. Once you are done, you will have to push the **Article** to your **Git repo.** 

**Alert:** If you do not have a Git repo connected, you cannot edit **Projects** on Stoplight. Learn how to connect Git accounts with your account: Connect Accounts

12. Click the **Push** button ****to upload all of your changes to Git. ****

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b8e13d70-7d6e-4557-9467-97cd9069775a/Screen_Shot_2021-02-12_at_3.06.12_AM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b8e13d70-7d6e-4557-9467-97cd9069775a/Screen_Shot_2021-02-12_at_3.06.12_AM.png)

12. Add in a **Commit Message**, specify the **Branch** and click **Push.** 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/508de7ed-6d86-4587-8556-eaaf2b1f0b9a/Screen_Shot_2021-02-12_at_3.05.37_AM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/508de7ed-6d86-4587-8556-eaaf2b1f0b9a/Screen_Shot_2021-02-12_at_3.05.37_AM.png)

**That's it. You just created your first article on Stoplight. ✍️**

## **What's Next?**

Now that you know how to create articles find out what next steps you can follow: 

1. **[Share Documentation](h.Creating-external-Documentation.md)** 
2. **[Create a Home Screen](Customizing-Docs/a.homescreen.md)** 
