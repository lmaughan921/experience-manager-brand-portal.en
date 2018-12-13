---
title: Publish presets, schema, and facets to Brand Portal
seo-title: Publish presets, schema, and facets to Brand Portal
description: null
seo-description: Learn how to publish presets, schema, and facets to Brand Portal.
uuid: d18f516c-fd15-4a6d-89a1-eeb399e91013
acrolinxdate: 2018-09-25T08 55 48.314-0400
acrolinxlastcheckedby: mgulati
acrolinxpagestatus: yellow
acrolinxreporturl: http //acrolinx.corp.adobe.com 8031/output/en/publish_schema_search_facets_presets_krs_workflow_a9d8be2d910fe9fc_1059_report.xml
acrolinxsentences: 63
acrolinxwords: 1130
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 6c01c486-228c-4da0-bd1a-c50291c8602c
isreadyforlocalization: false
index: y
internal: n
snippet: y
---

# Publish presets, schema, and facets to Brand Portal{#publish-presets-schema-and-facets-to-brand-portal}

The article delves into publishing image presets, metadata schemas, and custom search facets from AEM Author instance to Brand Portal. Publishing capability enables organizations to reuse the image presets, metadata schemas, and search facets created/modified at AEM Author instance thereby reducing duplicate efforts.

>[!NOTE]
>
>The capability to publish image presets, metadata schema, and search facets from AEM Author instance to Brand Portal is available AEM 6.2 SP1-CFP7 and AEM 6.3 SP 1-CFP 1 (6.3.1.1) onwards.

## Publish image presets to Brand Portal {#publish-image-presets-to-brand-portal}

Image presets are a set of sizing and formatting commands that are applied to the image at the time of image delivery. Image presets can be created and modified at Brand Portal. Alternatively, if AEM Author instance is running in dynamic media mode then users can create presets at the AEM Author and publish them to AEM Assets Brand Portal, and avoid re-creating the same presets at Brand Portal.  
Once the preset is created, it is listed as dynamic rendition on asset detail renditions rail and download dialogue.

>[!NOTE]
>
>If AEM Author instance is not running in Dynamic Media Mode (customer has not purchased Dynamic Media), then the  ptiff  rendition of the assets are not created at the time of upload. Image presets/ dynamic renditions work on ptiff of an asset, so if ptiff is not available on AEM Author then it is not available on the Brand Portal as well. As a result for this, no dynamic renditions are present in renditions rail of asset details page and download dialogue.

To publish image presets to Brand Portal:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/ click the Tools icon and navigate to **Assets **&gt; **Image Presets**.
1. Select the image preset or multiple image presets from the list of image presets and click/ tap **Publish to Brand Portal**.

![](assets/PublishPreset.png)

>[!NOTE]
>
>When users click **Publish to Brand Portal** the image presets are queued for publishing. Users are advised to monitor the log of the replication agents to confirm if the publish was successful.

To unpublish an image presets from Brand Portal:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **Assets **&gt; **Image Presets**.
1. Select an image preset, and select **Remove from Brand Portal** from the options available at the top.

## Publish metadata schema to Brand Portal  {#publish-metadata-schema-to-brand-portal}

Metadata schema describes the layout and properties that are displayed on the properties page of asset/ collections.

![](assets/Metadata-schema-editor.png)  ![](assets/Asset-properties.png)

If users have edited the default schema on AEM Author instance and are willing to use the same schema as default schema on the Brand Portal, they can simply publish the metadata schema forms to Brand Portal. In such a scenario, the default schema at Brand Portal is over-ridden by the default schemas published from AEM Author instance.

If users have created a custom schema on AEM Author instance, they can publish the custom schema to Brand Portal instead of re-creating the same custom schema there. Users can then apply this custom schema to any folder/ collection in Brand Portal.

>[!NOTE]
>
>Default schemas cannot be published to the Brand Portal if they are locked at the AEM instance (that is they are unedited).

![](assets/default-schema-form.png)

>[!NOTE]
>
>If a folder has a schema applied on AEM Author instance, the same schema must also exist on the Brand Portal to maintain the consistency in the asset properties page on AEM Author and Brand portal.

To publish a metadata schema from AEM Author instance to Brand Portal:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **Assets **&gt; **Metadata Schemas**.
1. Select a metadata schema, and select **Publish to Brand Portal** from the options available at the top.

>[!NOTE]
>
>When users click **Publish to Brand Portal,** the metadata schemas are queued for publishing. Users are advised to monitor the log of the replication agents to confirm if the publish was successful.

To unpublish a metadata schema from Brand Portal:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **Assets **&gt; **Metadata Schemas**.
1. Select a metadata schema, and select **Remove from Brand Portal** from the options available at the top.

## Publish search facets to Brand Portal {#publish-search-facets-to-brand-portal}

Search forms provide the capability of [faceted search](../using/brand-portal-search-facets.md) to users on Brand Portal. Search facets impart greater granularity to searches on Brand Portal. All the [predicates added](/content/help/en/experience-manager/6-4/assets/using/search-facets#AddingaPredicate) in the search form are available to users as search facets in search filters.

![](assets/Property-Predicate-removed-1.png)  ![](assets/Search-Form.png)

If you are willing to use custom search form **Assets Admin Search Rail **from AEM Author, then instead of re-creating the same form on Brand Portal you can publish the customized search form from AEM Author instance to Brand Portal.

>[!NOTE]
>
>Locked search form **Assets Admin Search Rail **on AEM Assets cannot be published to Brand Portal unless it is edited. Once edited and published to Brand Portal, this search form overrides the search form on Brand Portal.

To publish the edited search facet from AEM Author instance to Brand Portal:

1. Tap/click the AEM logo, and then go to **Tools** &gt; **General **&gt; **Search Forms**.
1. Select the edited search form, and select **Publish to Brand Portal**.

   >[!NOTE]
   >
   >When users click **Publish to Brand Portal,** the search facets are queued for publishing. Users are advised to monitor the log of the replication agents to confirm if the publish was successful.

To unpublish search forms from Brand Portal:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **General **&gt; **Search Forms**.
1. Select the search form, and select **Remove from Brand Portal** from the options available at the top.

>[!NOTE]
>
>The **Unpublish from Brand Portal** action leaves the default search form on Brand  Portal,  and does not restore to the last search form used before publishing.

### Limitations {#limitations}

1. Few search predicates are not applicable to search filters on the Brand Portal. When these search predicates are published as part of the search form from AEM Author instance to Brand Portal, they are filtered out. Users, therefore, see less number of predicates in the published form at the Brand Portal. See [search predicates applicable to filters on Brand Portal](../using/brand-portal-search-facets.md#Listofsearchpredicates).
1. For **Options **predicate, if a user is using any custom path to read options at AEM Author instance, it won't work at the Brand Portal. These additional paths and options are not published to Brand Portal with the search form. In this case, users can select the **Manual **option in **Add Options** within **Options Predicate** to add these options manually at Brand Portal.

![](assets/Options-Predicate-Manual.png)

