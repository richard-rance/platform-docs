## Custom Lint Rules

Validate your API files or enforce your organization's unique style. This guide will show you how. 

## **What are Custom Linting Rules?**

Working on **Stoplight studio,** you are alerted if you write invalid YAML, JSON, Markdown, or if your API descriptions are invalid OpenAPI, JSON Schema, etc. 

If you want to do more than just technical validation, such as a style guide to suggest naming conventions, missing information etc, you can do that by specifying **custom linting rules**. 

Customizing lint rules allow you to enable/disable built-in rules, add your own rules, and even change rule severities. You can enforce your organization's API style guides and surface errors at design time directly in the editor. 

> Note: Linting in Studio is powered by our open-source project **Spectral.**

## Configuring Custom Linting Rules

To configure custom linting rules:

1. Navigate to the project you want to customize the rules for.
2. Open the project, click on the **+** button at the top left of the screen, and select **Style Guide** from the dropdown to create a new linting file.

![V1.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/pM4sbcbU730)


3. For the new style guide specify the description format, inherited rulesets, and data format. Click **create** to get started. 

![V2.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/w78bzXKwrb4)


4. The new style guide will inherit all the standard rulesets for the description format you selected. 

![V3.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/zKXDejioy4A)


## **Modifying existing Rules**

For the rules that are inherited, you can enable/disable them or switch their severity. To do that:

1. Click the icon next to the rule, and pick one of the options from the dropdown that opens. 

![V4.png](https://stoplight.io/api/v1/projects/cHJqOjI/images/ejOQyCcuU5E)


Severity helps indiciate how the rule is applicable and range from:  

**Error:** Must have to reaach an acceptable state. 

**Warning:** Acceptable but may not produce desired results. 

**Information**: Missing information that might help complete an action. 

**Hint**: Indirect suggestion or a tip. 

A disabled rule will not be entertined. You can enable a previously disabled rule as according to need. 

## Adding a new Rule

To add a new rule to your style guide: 

![Video V5](../assets/V5.mov)


1. Switch to **code** view from **form** view, this will open an editor. 
2. Enter your custom rule. 
3. Once added, you would be able to see the rule under the section **Custom rules.** 
4. Push changes to workspace. 

A custom rule should look like this: 

```json
rules:
  my-rule-name:
    description: Tags must have a description.
    given: $.tags[*]
    severity: error
    then:
      field: description
      function: truthy
```

>Note: You can study how to define a rule in detail here: **Rules in Spectral** 

## **What's Next?**

Now that you know how to add a custom rule, as the next steps you can visit: 

- Custom Rulesets
- Custom Functions