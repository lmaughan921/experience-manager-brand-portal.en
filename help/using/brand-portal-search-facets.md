---
title: Use custom search facets
seo-title: Use custom search facets
description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
seo-description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
uuid: b228587a-3967-4f24-af63-551698f50ca9
acrolinxdate: 2018-08-16T07 50 58.355-0400
acrolinxlastcheckedby: mgulati
acrolinxpagestatus: yellow
acrolinxreporturl: http //acrolinx.corp.adobe.com 8031/output/en/brand_portal_search_facets_krs_workflow_a9d8be2d910fe9fc_102_report.xml
acrolinxsentences: 107
acrolinxwords: 1048
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 8d5315b2-307d-4c83-bf8c-09b96a9c4d67
isreadyforlocalization: false
index: y
internal: n
snippet: y
---

# Use custom search facets{#use-custom-search-facets}

Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.

Brand Portal supports [faceted search](../using/brand-portal-searching.md#Facetedsearchbyapplyingfilterstosearch) for granular searches of approved brand assets, which is possible due to [**Filters** panel](../using/brand-portal-searching.md#main-pars_text_55969420). Search facets are made available on Filters panel through **Search Form** in the admin tools. A default search form named Asset Admin Search Rail exists in Search Forms page in admin tools. However, Administrators can customize the default Filters panel by editing the default Search Form (Asset Admin Search Rail) by adding, modifying, or removing search predicates, thereby making the search functionality versatile.

You can use various search predicates to customize the **Filters** panel. For example, add the property predicate to search for assets that match a single property that you specify in this predicate. Add the options predicate to search for assets that match one or more values that you specify for a particular property. Add the date range predicate to search for assets created within a specified date range.

>[!NOTE]
>
>AEM allows organizations to [publish the customized search forms from AEM Author](/cf#publish-schema-search-facets-presets.html) to Brand Portal, instead of re-creating the same form on Brand Portal.

## Add a search predicate {#add-a-search-predicate}

To add a search predicate to the **Filters** panel:

1. To access administrative tools, click the AEM logo from the toolbar at the top.

   ![](assets/aemlogo.PNG)

1. From the administrative tools panel, click **Search Forms**. 

   ![](assets/Navigation-Panel-1.png)

1. In the **Search Forms** page, select **Assets Admin Search Rail**.

   ![](assets/search-forms-page.png)

1. On toolbar that appears at the top, click **Edit** to open the edit search form.

   ![](assets/edit-search-form-1.png)

1. In the **Edit Search Form** page, drag a predicate from the **Select Predicate** tab to the main pane. For example, drag **Property Predicate**.

   The **Property** field appears in the main pane and the **Settings** tab on the right displays property predicates.

   ![](assets/edit-search-form-properties.png)

   >[!NOTE]
   >
   >The header label in the **Settings** tab identifies the type of predicate you select.

1. In the **Settings** tab, enter a label, placeholder text, and description for the property predicate.

   >[!NOTE]
   >
   >Select **Ignore Case **if you want the asset search based on property values to be non-case sensitive. By default, the search for property values in search Filter is case-sensitive.

1. In the **Property Name** field, open property picker and select the property based on which the search is performed. Alternatively, enter a name for the property. For example, enter `jcr:content/metadata/dc:description` or `./jcr:content/metadata/dc:description`.

   ![](assets/search-form-property-picker.png)

1. Click **Done** to save the settings.
1. From the **Assets** user interface, click the overlay icon and choose **Filter** to navigate to the **Filters** panel. The **Property** predicate is added to the panel.

   ![](assets/Property-Filter-Panel.png)

1. Enter a description for the asset to be searched in the **Property** text box. For example, enter "Adobe." When you perform a search, assets with description matching "Adobe" are displayed in the search results.

## List of search predicates {#list-of-search-predicates}

Similar to the way you add a **Property** predicate, you can add the following predicates to the **Filters** panel:

<table border="1" cellpadding="0" cellspacing="0" width="100%"> 
 <tbody>
  <tr>
   <td width="19%"><p><strong>Predicate Name</strong></p> </td> 
   <td width="48%"><p><strong>Description</strong></p> </td> 
   <td width="31%"><p><strong>Properties</strong></p> </td> 
  </tr>
  <tr>
   <td>Path Browser</td> 
   <td><p>Search predicate to search assets at a particular location.</p> <p><strong>Note: </strong>For a logged-in user, path browser on Filter shows only the content structure of the folders (and their ancestors) shared with the user.</p> <p>Admin users can search assets in any folder by navigating to that folder using Path Browser.<br /> Whereas, non-admin users can search assets in a folder (accessible to them) by navigating to that folder in Path Browser.</p> </td> 
   <td>
    <ul> 
     <li>Field Label</li> 
     <li>Path</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td width="19%"><p>Property</p> </td> 
   <td width="48%">Search assets based on a particular metadata property.</td> 
   <td width="31%">
    <ul> 
     <li>Field Label</li> 
     <li>Placeholder</li> 
     <li>Property Name</li> 
     <li>Ignore Case</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>Multi-Value Property</td> 
   <td>Similar to property predicate but allows multiple input values, separated by a delimiter (default is COMMA[,]) assets matching any of the input values are returned in results.</td> 
   <td>
    <ul> 
     <li>Field Label</li> 
     <li>Placeholder</li> 
     <li>Property name</li> 
     <li>Delimiter Support</li> 
     <li>Ignore Case</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td width="19%"><p>Tags<br /> </p> </td> 
   <td width="48%"><p>Search predicate to search assets based on tags. You can configure the Path property to populate various tags in the Tags list.</p> <p><strong>Note:</strong> Administrators might need to change the path value, for example, <span class="code">/etc/tags/mac/&lt;tenant_id&gt;/&lt;custom_tag_namespace&gt;</span>, if they publish the search form from AEM, where the path does not include tenant information, for example, <span class="code">/etc/tags/&lt;custom_tag_namespace&gt;</span>.</p> </td> 
   <td width="31%">
    <ul> 
     <li>Field Label</li> 
     <li>Property name</li> 
     <li>Path</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>Path</td> 
   <td>Search predicate to search assets at a particular location.</td> 
   <td>
    <ul> 
     <li>Field Label</li> 
     <li>Path</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>Relative Date</td> 
   <td>Search predicate to search assets based on the relative date of their creation.</td> 
   <td>
    <ul> 
     <li>Field Label</li> 
     <li>Property name</li> 
     <li>Relative date</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>Range</td> 
   <td>Search predicate to search assets that lie within a specified range of property values. In the Filters panel, you can specify minimum and maximum property values for the range.</td> 
   <td>
    <ul> 
     <li>Field Label</li> 
     <li>Property name</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td><p>Date Range<br /> </p> </td> 
   <td width="48%">Search predicate to search assets created within a specified range for a date property. In the Filters panel, you can specify Start and End dates.<br /> </td> 
   <td width="31%">
    <ul> 
     <li>Field Label</li> 
     <li>Placeholder</li> 
     <li>Property name</li> 
     <li>Range text (From)</li> 
     <li>Range text (To)</li> 
     <li>Description<br /> </li> 
    </ul> </td> 
  </tr>
  <tr>
   <td><p>Date<br /> </p> </td> 
   <td width="48%">Search predicate for a slider-based search of assets based on a date property.<br /> </td> 
   <td width="31%">
    <ul> 
     <li>Field Label</li> 
     <li>Property name</li> 
     <li>Description<br /> </li> 
    </ul> </td> 
  </tr>
  <tr>
   <td><p>File Size<br /> </p> </td> 
   <td width="48%">Search predicate to search assets based on their size.<br /> </td> 
   <td width="31%">
    <ul> 
     <li>Field Label</li> 
     <li>Property name</li> 
     <li>Path</li> 
     <li>Description<br /> </li> 
    </ul> </td> 
  </tr>
  <tr>
   <td><p>Asset Last Modified</p> </td> 
   <td width="48%">Search predicate to search assets based on the last modified date.</td> 
   <td width="31%">
    <ul> 
     <li>Field Label</li> 
     <li>Property name</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>Approval Status</td> 
   <td>Search predicate to search assets based on approval metadata property. The default property name is <span class="code">dam
     <g class="gr_ gr_120 gr-alert gr_gramm gr_inline_cards gr_run_anim Style replaceWithoutSep" data-gr-id="120" id="120">
      :status
     </g></span>.</td> 
   <td>
    <ul> 
     <li>Field Label</li> 
     <li>Property name</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>Checkout Status</td> 
   <td>Search predicate to search assets based on the check-out status of an asset when it was published from AEM Assets.</td> 
   <td>
    <ul> 
     <li>Field Label</li> 
     <li>Property name</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>Checked Out By</td> 
   <td>Search predicate to search assets based on the user who has checked out the asset.</td> 
   <td>
    <ul> 
     <li>Field Label</li> 
     <li>Property name</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>Expiry Status</td> 
   <td>Search predicate to search assets based on the expiration status.</td> 
   <td>
    <ul> 
     <li>Field Label</li> 
     <li>Property name</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>Member of collection</td> 
   <td>Search predicate to search assets based on whether an asset is a part of a collection. </td> 
   <td>
    <ul> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
  <tr>
   <td>Hidden</td> 
   <td>This predicate is not explicitly visible to the end users and is used for any hidden constraints typically for restricting search results type to <span class="code">dam
     <g class="gr_ gr_116 gr-alert gr_gramm gr_inline_cards gr_run_anim Style replaceWithoutSep" data-gr-id="116" id="116">
      :Asset
     </g></span>.</td> 
   <td>
    <ul> 
     <li>Field Label</li> 
     <li>Property name</li> 
     <li>Description</li> 
    </ul> </td> 
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Do not use **Options Predicate**, **Publish Status Predicate**, and **Rating Predicate** as these predicates are not functional in Brand Portal.

## Delete a search predicate {#delete-a-search-predicate}

To delete a search predicate, follow these steps:

1. Click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.PNG)

1. From the administrative tools panel, click **Search Forms**. 

   ![](assets/Navigation-Panel-2.png)

1. In the **Search Forms** page, select **Assets Admin Search Rail**.

   ![](assets/search-forms-page.png)

1. On toolbar that appears at the top, click **Edit** to open the edit search form.

   ![](assets/edit-search-form-2.png)

1. In the **Edit Search Form** page, from the main pane, select the predicate you want to delete. For example, select **Property Predicate**.

   The **Settings** tab on the right displays property predicate fields.

1. To delete the property predicate, click the bin icon. On the **Delete Field** dialog box, click **Delete** to confirm the delete action.

   The **Property Predicate** field is removed from the main pane, and the **Settings** tab becomes empty.

   ![](assets/search-form-delete-predicate.png)

1. To save the changes, click **Done** in the toolbar.
1. From the **Assets** user interface, click the overlay icon and choose **Filter** to navigate to the **Filters** panel. The **Property** predicate is removed from the panel.

   ![](assets/Property-Predicate-removed.png)

