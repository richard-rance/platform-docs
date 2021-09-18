# Workspace Analytics
You can monitor activity and stats on your Stoplight workspace by configuring third party analytics tool. This guide will explain you how. 

## How does analytics work?

Analytics on Stoplight work with [Google Tag Manager.](https://tagmanager.google.com/) 

![image.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/oTsLwk8gVK4)

Google Tag Manger is a free tool that allows you to manage and deploy marketing tags, such as analytic scripts or tracking pixels, to your website. With Google Tag Manger, you can deploy several built-in tags including Google Analytics, CrazyEgg, Hotjar, LinkedIn Insight, Intercom and many more!

> **Note:** Analytics is only available on **[Stoplight Starter](https://stoplight.io/pricing/)** plan and above. 

## Configuring Workspace Analytics

Configuring Google Tag Manager is very easy. Before you begin anything you need to configure a [custom domain](../2.-workspaces/workspace-personalization/d.custom-domain.md). Once you have that, you can start following the instructions below. Google Tag Manger will be included with all of your configured marketing tags.

Here are the steps to get started:

1. [Create a free Google Tag Manager account](https://tagmanager.google.com/?hl=en#/admin/accounts/create) and copy your GTM ID (Eg. **`GTM-XXXXX-X`**).
2. Navigate to your Stoplight workspace settings and scroll to the **Custom Domain** section.

![Configure Analytics](https://stoplight.io/api/v1/projects/cHJqOjI/images/SiTthiOZBjo)

3. Enter your Google Tag Manager ID and hit save.

![configure Analytics](https://stoplight.io/api/v1/projects/cHJqOjI/images/0uau6ystiCg)


Now all you need to do is add marketing tags to your Google Tag Manager account, and they will be included when loading your custom domain. 

Check out this guide to [configure Google Analytics using Google Tag Manger.](https://support.google.com/tagmanager/answer/6107124?hl=en)) 

## **Limitations**

Stoplight blocks the use of any tags associated with the "customScripts" class in Google Tag Manager. These tags, such as the "Custom HTML" Tag, are capable of running JavaScript code provided by the user which could pose a security risk.

See the full list of tags associated with "customScripts": [https://developers.google.com/tag-manager/web/restrict](https://developers.google.com/tag-manager/web/restrict).

## What's Next?

After configuring analytics you can learn how to: 

- **[Hide Sign in button]()**
- **[Localize](url)**








