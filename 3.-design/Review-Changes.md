# **Review Changes**

The work you put in your API design or documentation might not always be ready to ship. To make sure your API projects work as intended, we recommend you review them first. Learn how to do that on Stoplight in this guide.

# **Why Review?**

Working as a solo developer you might be able to control what goes in your API project, but more often than less, it's multiple people and teams working on multiple projects, and quality control becomes a huge concern.

Sometimes the changes you make may cause things to break, other times they might not be consistent or easy to implement. All of which can be avoided by a simple review before being pushed to production. 

> **Note**: You can learn more about the API Reviewing process via our guide: **Review API Design**

## How to Review Changes?

Since Stoplight follows a Git based flow, reviewing changes on the platform works more or less like Git. We recommend you create a review branch, and push changes to it, once the changes are approved, then only merge them with the master branch. To create a **Review** branch: 

1. Navigate to and open your project on Stoplight **Studio**. 
2. On the top navbar of the studio, click on the **branch name**, next to he project name. 
3. Click **Switch Branches** from the dropdown that opens. 

![review1.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/6aPlevqaCKY)

4. If you already have a review branch in your Git project, select the branch. 
    
    
![review2.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/aolMrXoP4Cg)


3. If you do not have a **review branch**, type the name in the search bar and then press the "+" button to create a new branch. 

![review3.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/4h1NV65UTUw)


4. When you are done making changes, push them to the branch. 


5. For external members, make sure the branch is listed. Visit project settings make to make the branch publically available. 

![review4.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/ABybk81aYk4)


> **Note:** You can learn more about branch management by visiting our guide**: Switching Branches.** 

Once the reviewers have given feedback, you can push the changes to the main branch. 

## **What's Next?**

You now know how to run the review process on Stoplight. Next, you can take a look at: 

- [**API Security**](API-security.md)
- **Sharing Documentation**