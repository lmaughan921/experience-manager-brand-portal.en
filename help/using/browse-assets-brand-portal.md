---
title: Browsing assets on Brand Portal
seo-title: Browse assets on Brand Portal
description: Browse through assets, traverse asset hierarchies, and search assets, using different view options and UI elements on Brand Portal.
seo-description: Browse through assets, traverse asset hierarchies, and search assets, using different view options and UI elements on Brand Portal.
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
---

# Browsing assets on Brand Portal {#browsing-assets-on-brand-portal}

AEM Assets Brand Portal provides various capabilities and user interface elements that facilitate browsing through resources, traversing asset hierarchies, and searching assets while using different view options.

AEM logo in the AEM toolbar at the top facilitates admin users to access administrative tools panel.

![](assets/aemlogo.png) 
![](assets/admin-tools-panel-2.png) 
![](assets/bp_subheader.png)

Rail selector at the upper left in Brand Portal drops-down to expose options to navigate into asset hierarchies, streamline your search, and display resources.

![](assets/siderail-1.png)

You can view, navigate through, and select assets using any of the available views (Card, Column, and List) in the view selector at the upper right in Brand Portal.

![](assets/viewselector.png)

## Viewing and Selecting Resources {#viewing-and-selecting-resources}

Viewing, navigating, and selecting are each conceptually the same across all views, but have small variations in handling, depending on the view you are using.

You can view, navigate through, and select (for further action) your resources with any of the available views:

* Column View
* Card View  
* List View

### Card View

![](assets/card-view.png)

Card view displays information cards for each item at the current level. These cards provide the following details:

* A visual representation of the asset/folder.
* Type
* Title
* Name
* Date and time when asset was published to Brand Portal from AEM
* Size
* Dimensions

You can navigate down the hierarchy by tapping/clicking cards (taking care to avoid the quick actions) or up again by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

![](assets/cardquickactions.png)

#### Card view for non-admin users

Cards of folders, in Card View, display folder hierarchy information to non-admin users (Editor, Viewer, and Guest User). This functionality lets the users know the location of the folders, they are accessing, with respect to the parent hierarchy.
Folder hierarchy information is particularly helpful in differentiating the folders having names similar to other folders shared from a different folder hierarchy. If the non-admin users are not aware of the folder structure of the assets shared with them, assets /folders with similar names seem confusing.

* The paths shown on the respective cards are truncated to fit the card sizes. However, users can see the full path as a tool tipon hovering over the truncated path.

![](assets/folder-hierarchy1.png)

**Overview option to view Asset Properties**

Overview option is available to non-admin users (Editors, Viewers, Guest users) to view Asset Properties of selected assets/folders. The Overview option is visible:

1. In the toolbar at the top on selecting an asset/folder.
2. In the drop-down on selecting the Rail Selector.

On selecting the Overview option while an asset/folder is selected, users can see the title, path, and time of asset creation. Whereas, on asset detail page selecting Overview option lets the users see metadata of the asset.

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### View settings in card view

View Settings dialog opens on selecting View Settings from the view selector. It enables you to resize the asset thumbnails in the Card view. This way, you can personalize your view and control the number of thumbnails that is displayed.

![](assets/cardviewsettings.png)

### List View

![](assets/list-view.png)

The list view displays information for each resource at the current level. List view provides the following details:

* Thumbnail image of assets
* Name
* Title
* Locale
* Type
* Dimension
* Size
* Rating
* Folder path showing asset hierarchy<sup>*</sup>
* Date of publishing the asset on Brand Portal

&#42; Path column lets you easily identify asset location in the folder hierarchy. You can navigate down the hierarchy by tapping/clicking the resource name, and back up by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### View settings in list view

List view shows asset **Name** as the first column by default. Additional information, such as asset Title, Locale, Type, Dimensions, Size, Rating, Publish status are also shown. However, you can select the columns to be shown using View Settings.

![](assets/list-view-setting.png)

### Column View

 ![](assets/column-view.png)

Use the column view to navigate a content tree through a series of cascading columns. This view helps you visualize and traverse the asset hierarchy.

Selecting a resource in the first (leftmost) column displays child resources in the second column to the right. Selecting a resource in the second column displays child resources in the third column to the right, and so on.

You can navigate up and down in the tree by tapping or clicking the resource name or the chevron to the right of the resource name.

* The resource name and chevron are highlighted when tapped or clicked.
* Tapping or clicking the thumbnail selects the resource.
* When selected, a check mark is overlaid on the thumbnail and the resource name is highlighted.
* The details of the selected resource are shown in the final column.

When an asset is selected in column view, visual representation of the asset is displayed in the final column along with the following details:

* Title
* Name
* Dimensions
* Date and time when asset was published to Brand Portal from AEM
* Size
* Type
* More Details option, to go on the details page of the asset

<!--
Comment Type: draft

<h3>Selecting Resources</h3>
-->

<!--
Comment Type: draft

<p>Selecting a specific resource depends on a combination of the view and the device:</p>
-->

<!--
Comment Type: draft

<table border="1" cellpadding="1" cellspacing="0" width="100%">
<tbody>
<tr>
<td> </td>
<td>Select</td>
<td>Deselect</td>
</tr>
<tr>
<td>Column View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
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
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
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
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
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
-->

<!--
Comment Type: draft

<h4>Deselecting All</h4>
-->

<!--
Comment Type: draft

<p>In all cases, as you select items the count of the items selected is displayed at the upper right of the toolbar.</p>
<p>You can deselect all items and exit selection mode by clicking or tapping the X next to the count.</p>
-->

<!--
Comment Type: draft

<p>In all views, all items can be deselected by tapping escape on the keyboard if you are using a desktop device.</p>
-->

## Content Tree {#content-tree}

In addition to these views, use the tree view to drill down the asset hierarchy while you view and select desired assets or folders.

To open the tree view, tap/click the rail selector at upper left and select the **Content tree** from the menu.

![](assets/contenttree.png)

From the content hierarchy, navigate to the desired asset.

![](assets/content-tree.png)

## Asset Details {#asset-details}

Asset detail page lets you view an asset, download, share asset's link, move it to a collection, or view its properties page. It also allows you to navigate through the details page of other assets of the same folder in succession.

![](assets/asset-detail.png)

To overview the asset's metadata, or view its various renditions, use the rail selector on asset detail page.

![](assets/asset-overview.png)

You can view all the available renditions of the asset on asset details page, and select a rendition to preview it.

![](assets/renditions.png)

To open the asset properties page, use *Properties (p)* option on the top bar.

![](assets/asset-properties.png)

You can also view a list of all its related assets (source or derived assets on AEM) on an asset's properties page, as asset relationship is also published from AEM to Brand Portal.
