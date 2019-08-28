---
title: Publish presets, schema, and facets to Brand Portal
seo-title: Publish presets, schema, and facets to Brand Portal
description: Learn how to publish presets, schema, and facets to Brand Portal.
seo-description: Learn how to publish presets, schema, and facets to Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
---

# Publish presets, schema, and facets to Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

The article delves into publishing image presets, metadata schemas, and custom search facets from [!DNL AEM] Author instance to [!DNL Brand Portal]. Publishing capability enables organizations to reuse the image presets, metadata schemas, and search facets created/modified at [!DNL AEM] Author instance thereby reducing duplicate efforts.

>[!NOTE]
>
>The capability to publish image presets, metadata schema, and search facets from [!DNL AEM] Author instance to [!DNL Brand Portal] is available [!DNL AEM 6.2 SP1-CFP7] and [!DNL AEM 6.3 SP 1-CFP 1 (6.3.1.1)] onwards.

## Publish image presets to Brand Portal {#publish-image-presets-to-brand-portal}

Image presets are a set of sizing and formatting commands that are applied to the image at the time of image delivery. Image presets can be created and modified at [!DNL Brand Portal]. Alternatively, if [!DNL AEM] Author instance is running in dynamic media mode then users can create presets at the [!DNL AEM] Author and publish them to [!DNL AEM Assets Brand Portal], and avoid re-creating the same presets at [!DNL Brand Portal].  
Once the preset is created, it is listed as dynamic rendition on asset detail renditions rail and download dialogue.

>[!NOTE]
>
>If [!DNL AEM] Author instance is not running in [!DNL Dynamic Media] Mode (customer has not purchased [!DNL Dynamic Media]), then the [!UICONTROL Pyramid TIFF]  rendition of the assets are not created at the time of upload. Image presets or dynamic renditions work on [!UICONTROL Pyramid TIFF] of an asset, so if [!UICONTROL Pyramid TIFF] is not available on [!DNL AEM] Author instance then it is not available on [!DNL Brand Portal] as well. As a result of this, no dynamic renditions are present in renditions rail of asset details page and download dialogue.

To publish image presets to [!DNL Brand Portal]:

1. In [!DNL AEM] Author instance, tap/ click the [!DNL AEM] logo to access the global navigation console and tap/ click the Tools icon and navigate to **[!UICONTROL Assets]** &gt; **[!UICONTROL Image Presets]**.
2. Select the image preset or multiple image presets from the list of image presets and click/ tap **[!UICONTROL Publish to Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>When users click **[!UICONTROL Publish to Brand Portal]** the image presets are queued for publishing. Users are advised to monitor the log of the replication agents to confirm if the publish was successful.

To unpublish an image preset from [!DNL Brand Portal]:

1. In [!DNL AEM] Author instance, tap/ click the [!DNL AEM] logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets]** &gt; **[!UICONTROL Image Presets]**.
2. Select an image preset, and select **[!UICONTROL Remove from Brand Portal]** from the options available at the top.

## Publish metadata schema to Brand Portal  {#publish-metadata-schema-to-brand-portal}

Metadata schema describes the layout and properties that are displayed on the properties page of asset/ collections.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

If users have edited the default schema on [!DNL AEM] Author instance and are willing to use the same schema as default schema on the [!DNL Brand Portal], they can simply publish the metadata schema forms to [!DNL Brand Portal]. In such a scenario, the default schema at [!DNL Brand Portal] is over-ridden by the default schemas published from [!DNL AEM] Author instance.

If users have created a custom schema on [!DNL AEM] Author instance, they can publish the custom schema to [!DNL Brand Portal] instead of re-creating the same custom schema there. Users can then apply this custom schema to any folder/ collection in [!DNL Brand Portal].

>[!NOTE]
>
>Default schemas cannot be published to the [!DNL Brand Portal] if they are locked at the [!DNL AEM] instance (that is they are unedited).

![](assets/default-schema-form.png)

>[!NOTE]
>
>If a folder has a schema applied on [!DNL AEM] Author instance, the same schema must also exist on the [!DNL Brand Portal] to maintain the consistency in the asset properties page on [!DNL AEM] Author and [!DNL Brand portal].

To publish a metadata schema from [!DNL AEM] Author instance to [!DNL Brand Portal]:

1. In [!DNL AEM] Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets]** &gt; **[!UICONTROL Metadata Schemas]**.
2. Select a metadata schema, and select **[!UICONTROL Publish to Brand Portal]** from the options available at the top.

>[!NOTE]
>
>When users click **[!UICONTROL Publish to Brand Portal]**, the metadata schemas are queued for publishing. Users are advised to monitor the log of the replication agents to confirm if the publish was successful.

To unpublish a metadata schema from [!DNL Brand Portal]:

1. In [!DNL AEM] Author instance, tap/ click the [!DNL AEM] logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets]** &gt; **[!UICONTROL Metadata Schemas]**.
2. Select a metadata schema, and select **[!UICONTROL Remove from Brand Portal]** from the options available at the top.

## Publish search facets to Brand Portal {#publish-search-facets-to-brand-portal}

Search forms provide the capability of [faceted search](../using/brand-portal-search-facets.md) to users on [!DNL Brand Portal]. Search facets impart greater granularity to searches on [!DNL Brand Portal]. All the [predicates added](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) in the search form are available to users as search facets in search filters.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

If you are willing to use custom search form **[!UICONTROL Assets Admin Search Rail]** from [!DNL AEM] Author instance, then instead of re-creating the same form on [!DNL Brand Portal] you can publish the customized search form from [!DNL AEM] Author instance to [!DNL Brand Portal].

>[!NOTE]
>
>Locked search form **[!UICONTROL Assets Admin Search Rail]** on AEM Assets cannot be published to [!DNL Brand Portal] unless it is edited. Once edited and published to [!DNL Brand Portal], this search form overrides the search form on [!DNL Brand Portal].

To publish the edited search facet from [!DNL AEM] Author instance to [!DNL Brand Portal]:

1. Tap/click the [!DNL AEM] logo, and then go to **[!UICONTROL Tools]** &gt; **[!UICONTROL General]** &gt; **[!UICONTROL Search Forms]**.
2. Select the edited search form, and select **[!UICONTROL Publish to Brand Portal]**.

   >[!NOTE]
   >
   >When users click **[!UICONTROL Publish to Brand Portal]**, the search facets are queued for publishing. Users are advised to monitor the log of the replication agents to confirm if the publish was successful.

To unpublish search forms from [!DNL Brand Portal]:

1. In [!DNL AEM] Author instance, tap/ click the [!DNL AEM] logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL General]** &gt; **[!UICONTROL Search Forms]**.
2. Select the search form, and select **[!UICONTROL Remove from Brand Portal]** from the options available at the top.

>[!NOTE]
>
>The **[!UICONTROL Unpublish from Brand Portal]** action leaves the default search form on Brand  Portal,  and does not restore to the last search form used before publishing.

### Limitations {#limitations}

1. Few search predicates are not applicable to search filters on the [!DNL Brand Portal]. When these search predicates are published as part of the search form from [!DNL AEM] Author instance to [!DNL Brand Portal], they are filtered out. Users, therefore, see less number of predicates in the published form at the [!DNL Brand Portal]. See [search predicates applicable to filters on Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

2. For [!UICONTROL Options] predicate, if a user is using any custom path to read options at AEM Author instance, it won't work at the Brand Portal. These additional paths and options are not published to Brand Portal with the search form. In this case, users can select the **[!UICONTROL Manual]** option in **[!UICONTROL Add Options]** within **[!UICONTROL Options Predicate]** to add these options manually at [!DNL Brand Portal].

![](assets/options-predicate-manual.png)
