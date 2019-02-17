---
title: Dynamic video support on Brand Portal
seo-title: Dynamic video support on Brand Portal
description: Dynamic video support on Brand Portal
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
index: y
internal: n
snippet: y
---

# Dynamic video support on Brand Portal{#dynamic-video-support-on-brand-portal}

Brand Portal allows previewing, playing, and downloading videos from the portal and shared links. Also, you can play Dynamic Media encodes of the video assets on asset details page, and download the encodes from the portal, and shared links. To enable preview, play, and download of video assets (published from AEM Author instance) adaptively from the cloud on Brand Portal, you need to set up the appropriate [Dynamic Media configurations](../using/dynamic-video-brand-portal.md#main-pars-header) in Video configurations page.

>[!NOTE]
>
>To work with rich video assets and to publish them to Brand Portal, make sure that your AEM Author instance is set up on Dynamic Media Hybrid mode.

## Prerequisites {#prerequisites}

* AEM Author instance is set up on [Dynamic Media Hybrid mode](/content/help/en/experience-manager/6-4/assets/using/config-dynamic).
* Video assets are published from AEM Author instance to Brand Portal.
* [Dynamic Media configurations](../using/dynamic-video-brand-portal.md#main-pars-header) are set up on Brand Portal.

## How are dynamic videos played? {#how-are-dynamic-videos-played}

If **Dynamic Media configuration **(video service URL (DM Gateway URL) and tenant-specific registration ID) is set up on Brand Portal, the dynamic video is fetched from Dynamic Media Gateway and video encodes can be previewed and played without delay and distortion in quality.

The binaries of dynamic encodes of videos are not stored in the repository (*/crx/de*) and are fetched from the cloud, which is Dynamic Media Gateway based on Registration ID you specify in the configuration.   
Once you configure Dynamic Media settings:

* Videos are previewed in Card view.
* All the Video encodes are played in asset detail page.
* Video renditions are downloaded from Brand Portal and Shared link.

>[!NOTE]
>
>Video viewers and viewer presets are not supported in Brand Portal. Videos are previewed and played on the default viewers in Brand Portal.

## Configure Dynamic Media settings {#configure-dynamic-media-settings}

**Video** configuration available in the administrative tools panel lets you navigate to the **Edit Dynamic Media Configuration **page, to add/ edit the Dynamic Media gateway settings from where the video encodes are fetched to preview and play in Brand Portal.

To set up Dynamic Media configurations on specific tenants:

1. On Brand Portal, select the AEM logo to access administrative tools from the toolbar at the top.
1. From the administrative tools panel, select **Video** to access the **Edit Dynamic Media Configuration** page.

   ![](assets/edit-dynamic-media-config.png)

1. Specify **Registration ID** and **Video Service URL** (DM-Gateway URL), which are the same as in your AEM Author instance.

   To copy the Dynamic Media Configuration (video service URL (DM Gateway URL) and registration ID so that dynamic video is fetched from DM Gateway) from AEM Author instance:

    1. In your AEM Author instance, go to **Tools** and select **Cloud Services**.
    1. Open **Dynamic Media Configuration (Pre 6.3) **to access** Dynamic Media Configuration Browser (Pre 6.3).**
    1. Copy the **Registration ID **and **Video Service URL**.

1. Select **Save** to save the configuration.

