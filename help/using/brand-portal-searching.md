---
title: Search assets on Brand Portal
seo-title: Asset searching and saved search on AEM Brand Portal
description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
index: y
internal: n
snippet: y
---

# Search assets on Brand Portal {#search-assets-on-brand-portal}

Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and faceted search that uses filters to help you further narrow down your search. You can also save your searches as smart collections for the future.

## Search assets using Omnisearch {#search-assets-using-omnisearch}

To search for assets on Brand Portal:

1. From the toolbar, click the **Search** icon, or press the "**/**" key to launch Omnisearch.

   ![](assets/omnisearchicon-1.png)

2. In the search box, type a keyword for the assets you want to search.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >At least 3 characters are required in omnisearch for search suggestions to appear.

3. Select from the related suggestions that appear in the drop-down list to quickly access relevant assets.

   ![](assets/assets-search-result.png)

   Asset search using omnisearch

## Search using facets in Filters panel {#search-using-facets-in-filters-panel}

Search facets in the Filters panel add granularity to your search experience and make the search functionality efficient. Search facets use multiple dimensions (predicates) that enable you to perform intricate searches. You can easily drill down to the desired level of detail for a more focused search.

For example, if you are looking for an image, you can choose whether you want a bitmap or a vector image. You can reduce the scope of search further by specifying the MIME type for the image in the File Type search facet. Similarly, when searching for documents, you can specify the format, for example, PDF or MS Word format.

![Filters panel in Brand Portal](assets/file-type-search.png "Filters panel in Brand Portal")

The Filters panel includes a few standard facets, such as- Path Browser, File Type, File Size, Status, and Orientation. However, you can [add custom search facets](../using/brand-portal-search-facets.md) or remove specific search facets from the **Filters** panel by adding or removing predicates in the underlying Search Form. See the list of the available and usable [search predicates on Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

To apply filters to your search, using the available [search facets](../using/brand-portal-search-facets.md):

1. Click the overlay icon and select **Filter**.

   ![](assets/selectorrail.png)

2. From the **Filters** panel on the left, select the appropriate options to apply the relevant filters.
   For example, use the following standard filters:

    * **Path Browser** to search assets in a specific directory. The default search path of the predicate for Path Browser is */content/dam/mac/&lt;tenant-id&gt;/*, which can be configured by editing the default search form.

   >[!NOTE]
   >
   >To non-admin users, Path Browser in Filter panel shows only the content structure of the folders (and their ancestor folders) shared with them.  
   >To admin users, Path Browser allows navigating to any folder in Brand Portal.

    * **File Type** to specify the type (image, document, multimedia, archive) of asset file you are looking for. Further, you can narrow down the scope of your search, for example, specify the MIME type (Tiff, Bitmap, GIMP Images) for image or format (PDF or MS Word) for the documents.
    * **File Size** to search for assets based on their size. You can specify the lower and upper limits for the size range to narrow down your search and specify the unit of measure to search.
    * **Status** to search for assets based on asset statuses, such as Approval (Approved, Changes Requested, Rejected, Pending) and Expiration.
    * **Average Rating** to search for assets based on the rating of the assets.
    * **Orientation** to search for assets based on the orientation (horizontal, vertical, square) of the assets.
    * **Style** to search for assets based on the style (colored, monochrome) of the assets.
    * **Video Format** to search for video assets based on their format (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).

   You can use [custom search facets](../using/brand-portal-search-facets.md) in the Filters panel by editing the underlying Search Form.

    * **Property Predicate** if used in the search form, lets you search for assets that match a metadata property to which the predicate is mapped.  
      For example, if Property Predicate is mapped to `jcr:content /metadata/dc:title`, you can search assets based on their title.  
      The Property Predicate supports text searches for:  

      **Partial phrases**
      To allow the asset search using partial phrases in property predicate, enable the **Partial Search** checkbox in Search Form.  
      This allows you to search for the desired assets even if you do not specify the exact words/ phrases used in the asset metadata.  
      You can:
          1. Specify a word occurring in your searched phrase in the facet in Filters panel. For example, if you search for the term **climb** (and Property Predicate is mapped to `dc:title` property), then all the assets with the word **camp** in their title phrase are returned.
          2. Specify a part of the word, occurring in your searched phrase, along with wildcard character (&#42;) to fill the gaps.
          For example, searching for:
          **climb&#42;** returns all the assets having words beginning with the characters "climb" in their title phrase.
          **&#42;climb** returns all the assets having words ending with characters "climb" in their title phrase.
          **&#42;climb&#42;** returns all the assets having words comprising the characters "climb" in their title phrase.  
      **Non-case sensitive text**
      To allow non-case sensitive search in property predicate,enable the **Ignore Case** checkbox in Search Form. By default, the text search on property predicate is case-sensitive.

   >[!NOTE]
   >
   >On selecting **Partial Search** checkbox, **Ignore Case** is selected by default.

   ![](assets/wildcard-prop-1.png)

   The search results are displayed according to the filters applied, along with the search results count.

   ![](assets/omnisearch-with-filters.png)

   Asset search result with search result count

3. You can easily navigate to an item from the search result, and return to the same search result using the back button in your browser without having to re-run the search query.

## Save your searches as smart collection {#save-your-searches-as-smart-collection}

You can save the search settings as a smart collection to be able to quickly repeat the same search without having to redo the same settings later.

To save the search settings as a smart collection:

1. Tap/ click **Save Smart Collection** and provide a name for the smart collection.

   To make the smart collection accessible to all users, select **Public**. A message confirms that the smart collection was created and added to the list of your saved searches.

   >[!NOTE]
   >
   >Non-admin users can be restricted from making smart collections public, to avoid having a huge number of public smart collections created by non-admin users on organization's Brand Portal. Organizations can disable the **Allow public smart collections creation** configuration from **General** settings available in admin tools panel.

   ![](assets/save_smartcollectionui.png)

1. To save the smart collection in a different name, and select or clear the **Public** checkbox, click **Edit Smart Collection**.

   ![](assets/edit_smartcollection.png)

1. On the **Edit Smart Collection** dialog box, select **Save As** and enter a name for the smart collection. Click **Save**.

   ![](assets/saveas_smartsearch.png)
