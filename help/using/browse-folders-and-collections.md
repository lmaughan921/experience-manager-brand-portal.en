---
title: Browse folders and collections
seo-title: Browse folders and collections
description: The elements in the AEM Assets Brand Portal header facilitate browsing through assets, traversing asset hierarchies, and asset search, while utilizing different view options.
seo-description: The elements in the AEM Assets Brand Portal header facilitate browsing through assets, traversing asset hierarchies, and asset search, while utilizing different view options.
page-status-flag: never-activated
uuid: aa06c36a-a1cc-42ed-8e71-a51e5c753aa3
contentOwner: bdhar
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: visits
discoiquuid: eb63bacf-7faa-446a-83c4-7833fa181924
index: y
internal: n
snippet: y
---

# Browse folders and collections{#browse-folders-and-collections}

The elements in the AEM Assets Brand Portal header facilitate browsing through assets, traversing asset hierarchies, and asset search, while utilizing different view options.

The Brand Portal header:

![](assets/bp_subheader.png)

Callouts: Rail selector, Breadcrumbs, View selector

You can view, navigate through, and select assets using any of the available views (Card, Column, and List) in the view selector.

In List view, the Select icon appears when you hover the mouse icon over the thumbnail before the names of the assets/folder in the list.

Similar to List view, the Select icon appears when you hover the mouse icon over the thumbnail before the names of the assets/folder in Column view.

For more information, see [Viewing and Selecting your Resources](/content/help/en/experience-manager/6-3/sites/authoring/using/basic-handling#main-pars_title_14).

## Viewing and Selecting Resources {#viewing-and-selecting-resources}

Viewing, navigating, and selecting are each conceptually the same across all views, but have small variations in handling, dependent on the view you are using.

You can view, navigate through, and select (for further action) your resources with any of the available views, each of which can be selected by the icon at the top right:

* [Column View](#columnview)
* [Card View](#cardview)  

* [List View](#listview)

>[!NOTE]
>
>By default, AEM Assets does not display the original renditions of assets in the UI as thumbnails in any of the views. If you are an administrator, you can use overlays to configure AEM Assets to display original renditions as thumbnails.

### Selecting Resources {#selecting-resources}

Selecting a specific resource is dependent on a combination of the view and the device:

<table border="1" cellpadding="1" cellspacing="0" width="100%"> 
 <tbody>
  <tr>
   <td> </td> 
   <td>Select</td> 
   <td>Unselect</td> 
  </tr>
  <tr>
   <td>Column View<br /> </td> 
   <td>
    <ul> 
     <li>Desktop:<br /> Click the thumbnail</li> 
     <li>Mobile device:<br /> Tap the thumbnail</li> 
    </ul> </td> 
   <td>
    <ul> 
     <li>Desktop:<br /> Click the thumbnail</li> 
     <li>Mobile device:<br /> Tap the thumbnail</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>Card View<br /> </td> 
   <td>
    <ul> 
     <li>Desktop:<br /> Mouseover, then use the checkmark quick action</li> 
     <li>Mobile device:<br /> Tap-and-hold the card</li> 
    </ul> </td> 
   <td>
    <ul> 
     <li>Desktop:<br /> Click the card</li> 
     <li>Mobile device:<br /> Tap the card</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>List View</td> 
   <td>
    <ul> 
     <li>Desktop:<br /> Click the thumbnail</li> 
     <li>Mobile device:<br /> Tap the thumbnail</li> 
    </ul> </td> 
   <td>
    <ul> 
     <li>Desktop:<br /> Click the thumbnail</li> 
     <li>Mobile device:<br /> Tap the thumbnail</li> 
    </ul> </td> 
  </tr>
 </tbody>
</table>

#### Deselecting All {#deselecting-all}

In all cases as you select items, the count of the items selected is displayed at the top-right of the toolbar.

You can deselect all items and exit selection mode by clicking or tapping the X next to the count.

In all views, all items can be deslected by tapping escape on the keyboard if you are using a desktop device.

### Column View {#column-view}

Use the column view to navigate a content tree through a series of cascading columns. This view helps you visualize and traverse the tree structure of your website.

Selecting a resource in the first (leftmost) column displays child resources in the second column to the right. Selecting a resource in the second column displays child resources in the third column to the right, and so on.

You can navigate up and down in the tree by tapping or clicking on the resource name or the chevron to the right of the resource name.

* The resource name and chevron will be highlighted when tapped or clicked.

* The children of the clicked/tapped resource are displayed in the column to the right of the clicked/tapped resource.
* If you tap or click on a resource name that has no children, its details will be displayed in the final column.

Tapping or clicking on the thumbnail selects the resource.

* When selected, a checkmark will be overlaid on the thumbnail and the resource name will be highlighted as well.
* The details of the selected resource will be shown in the final column.

When a page is selected in column view, the selected page is displayed in the final colum along with the following details:

* Page title
* Page name (part of the page's URL)
* Template the page is based on
* Last modified date
* Last user to modify page
* Page language
* Publication status

### Card View {#card-view}

Card view displays information cards for each item at the current level. These provide information such as:

* A visual representation of the page content.
* The page title.
* Important dates (such as last edited, last published).
* If the page is locked, hidden or part of a livecopy.  
* If appropriate, when you are required to take action as part of a workflow.

    * Markers that indicate required actions may be related to entries in your [Inbox](/content/help/en/experience-manager/6-3/sites/authoring/using/inbox).

[Quick actions](#quickactions) are also available in this view such as selection and common actions such as edit.

You can navigate down the tree by tapping/clicking on cards (taking care to avoid the quick actions) or up again by using the [breadcrumbs in the header](/content/help/en/experience-manager/6-3/sites/authoring/using/basic-handling#main-pars_title_21).

### List View {#list-view}

The list view lists information for each resource at the current level.

You can navigate down through the tree by tapping/clicking on the resource name and back up by using the [breadcrumbs in the header](/content/help/en/experience-manager/6-3/sites/authoring/using/basic-handling#main-pars_title_21).

To easily select all items in the list, use the checkbox at the top-left of the list.

* When all items in the list are selected, this checkbox appears checked.

    * Click or tap the checkbox to deselect all.

* When only some items are selected, it appears with a minus sign.

    * Click or tap the checkbox to select all.
    * Click or tap the checkbox again to deselect all.

Select the columns to be shown using **View Settings **option located under the Views button. The following columns are available for display:

* **Name** - Page name, which can be useful in a multilingual authoring environment since it is part of the page's URL and does not change regardless of language
* **Modified** - Last modified date and last modified by user
* **Published** - Publication status
* **Template** - Template on which the page is based
* **Page analytics**
* **Unique visitors**
* **Time on page**

By default the **Name** column is shown, which makes up part of the URL for the page. In some cases the author might need to access pages that are in a different language and seeing the name of the page (which usually is unchanging) can be of great help if the author does not know the language of the page.

Change the order of items using the dotted vertical bar at the far right of each item in the list.

Click or tap on the vertical selection bar and drag the item to a new position in the list.
