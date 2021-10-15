# Navigation

Great documentation guides readers to where they need to go instead of making them search.

Start by setting up the table of contents in the [project sidebar](Sidebar/d.table-of-contents.md). Next setup deep links using the below best practices. 


## From external page to markdown page

Simply copy the link from your browser when not in edit mode.

You may edit the title text at the end to make it more memerable without breaking the link. Only the hash really matters. The default title is set based on the link in the table of contents that was clicked.

The hash is generated based on the path to where the file is saved relitive to the root of the project. The hash does not change between versions when working with multiple branches. If you reorganize your files you will want to [configure redirects](e2.configure-redirects.md). 


## From markdown page to markdown page
When linking between pages you use the standard markdown syntax and relitive paths from the current page. 

For example `[API Governance](../5.-governance/b.getting-started-with-api-governance.md)`

Using absolute links from the root of the project is not recommended as it does not play well with multiple branches. //TODO Confirm this is still a problem with the new router.


## From API reference to markdown Page

## From markdown page to API reference

## Linking between versions