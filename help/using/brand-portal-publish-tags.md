---
title: Publish tags to Brand Portal
seo-title: Publish tags to Brand Portal
description: Learn how to publish tags from AEM Assets to Brand Portal.
seo-description: Learn how to publish tags from AEM Assets to Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
---

# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

Learn how to publish tags from AEM Assets to Brand Portal.

Tags are useful in organizing assets and enhance the searchability of assets to which they are associated. Tags can be thought of as keywords or labels (metadata) that are attached with assets, and allow assets to be quickly found as the result of a search. To know how to assign tags to assets in AEM Assets, refer [use tags to organize assets](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Tags (associated with assets and collections in AEM) are auto-published to Brand Portal when the assets (and collections) with associated tags are published to Brand Portal. The published tags are helpful in enabling the searches to find the associated assets.

>[!NOTE]
>
>It is, however, recommended to exclusively publish tags to Brand Portal before publishing the assets (and collections) with which the tags are associated. This ensures faster publishing of the assets (and collections) to Brand Portal.

## Manage tags {#manage-tags}

You can use the pre-existing tags to attach to an asset or create new tags from AEM Tags console (**[!UICONTROL Tools | Tagging | AEM Tags]**). In both the scenarios you must first publish the tags to Brand Portal and then associate them with appropriate assets.

To create tags on AEM, publish the tags on Brand Portal, and associate the tags with appropriate assets (or collections), follow these steps:

1. **Create Tags**
Sign in to AEM Author instance with administrative privileges, and access **[!UICONTROL AEM Tags]** console from global navigation:

   1. Select **[!UICONTROL Tools]**

   2. Select **[!UICONTROL General]**

   3. Select **[!UICONTROL Tagging]**

2. Select **[!UICONTROL Create]** and then select **[!UICONTROL Create Tag]** option.
3. Specify:

    * **[!UICONTROL Title]**
      *(required)* A display title for the tag.
    * **[!UICONTROL Name]**
      *(required)* A name for the tag. If not specified, a valid node name is created from the Title. See [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
    * **Description**
      *(optional)* A description of the tag.
    * **Tag Path**
      JCR path of the tag.

4. Select **[!UICONTROL Submit]** to create the tag.

   Once you have created a tag on AEM instance, the tag will be available to be attached to an asset (using Properties section or Manage Tags section of that asset).

5. **Publish the tag to Brand Portal**.

   Go to **[!UICONTROL AEM Tags]** console ([!UICONTROL Tools | Tagging | AEM Tags]), select the desired tag and Publish to Brand Portal.

6. **Attach the tag to an asset (or collection)**.

   Select an asset (or collection), and attach the desired tag using Properties section or Manage Tags section of that asset. To know more about how to assign tags to assets in AEM Assets, refer [use tags to organize assets](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

7. **Publish assets (or collections) to Brand Portal**.  
   When you publish an asset (or collection) to Brand Portal, the attached tag is also available on Brand Portal.

   To see the attached tag on the respective asset (or collection) in Brand Portal, log in to Brand Portal and select the asset, under Properties section you will see the attached Tag.

## Search Promote {#search-promote}

AEM Assets Brand Portal allows you to make specific assets come as the top results for searches based on a keyword tag.

To elevate an asset for a search keyword, follow these steps:

1. Open the **[!UICONTROL Properties]** page of an asset on AEM author instance.
2. Go to **[!UICONTROL Advanced]** tab.
3. In **[!UICONTROL Search Promote]** within **[!UICONTROL Elevate for search keywords]** section, select **[!UICONTROL Add]** to add the search keywords or tags.

   ![](assets/search-promote.png)

4. Save the changes.
5. Publish the asset to Brand Portal.
6. Log in to Brand Portal. View **[!UICONTROL Advanced]** tab in **[!UICONTROL Properties]** section of the asset.
Note that the **[!UICONTROL Search Promote]** keyword is also visible in the Properties of that asset.
