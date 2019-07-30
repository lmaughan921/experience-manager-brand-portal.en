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
---

# Dynamic video support on Brand Portal {#dynamic-video-support-on-brand-portal}

Preview and play videos adaptively on Brand Portal with Dynamic Media support. Also, download the dynamic renditions from the portal and shared links.
Brand Portal users can:

* Preview videos in Asset Details page, Card View, and link share preview page.
* Play video encodes on Asset Details page.
* View dynamic renditions in Renditions tab on Asset Details page.
* Download video encodes and folders containing videos.

>[!NOTE]
>
>To work with videos and to publish them to Brand Portal, make sure that your AEM Author instance is set up either on Dynamic Media Hybrid mode or Dynamic Media Scene 7 mode.

To preview, play, and download videos, Brand Portal exposes the following two configurations to administrators:

* [Dynamic Media Hybrid configuration](#configure-dm-hybrid-settings)
If AEM Author instance is running on dynamic media Hybrid mode.
* [Dynamic Media Scene 7 configuration](#configure-dm-scene7-settings)
If AEM Author instance is running on dynamic media-Scene 7 mode.
Set either of these configurations based on the configurations you set in your AEM Author instance with which Brand Portal tenant is replicated.

>[!NOTE]
>
>Dynamic videos are not supported on Brand Portal tenants integrated with AEM Author running on Scene7Connect runmode.

## How are dynamic videos played? {#how-are-dynamic-videos-played}

![Video encodes are fetched from cloud](assets/VideoEncodes.png)

If Dynamic Media configurations ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) or [Scene 7](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configurations) are set up on Brand Portal, the dynamic renditions are fetched from Scene 7 server. Video encodes are, therefore, previewed and played without delay and distortion in quality.

As video encodes are not stored in Brand Portal repository and are fetched from Scene 7 server, ensure that the Dynamic Media configurations on AEM Author Instance and Brand Portal are the same.

>[!NOTE]
>
>Video viewers and viewer presets are not supported in Brand Portal. Videos are previewed and played on the default viewers in Brand Portal.

## Prerequisites {#prerequisites}

To work with dynamic videos on Brand Portal, make sure to:

* **Start up AEM Author on DM (Dynamic Media) mode**
Start up the AEM Author instance (with which Brand Portal is integrated) either on [Dynamic Media Hybrid mode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) or [Dynamic Media Scene 7 mode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configure DM cloud services on AEM Author**
Based on the DM mode AEM Author is running on, set either of [Dynamic Media cloud services](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) or [Scene 7 cloud services](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) on AEM Author from **Tools** > **Cloud Services** > **Dynamic Media**.  
* **Configure DM on Brand Portal**
Based on the DM cloud configurations on AEM Author, configure [Dynamic Media settings](#configure-dm-hybrid-settings) or [Scene 7 settings](#configure-dm-scene7-settings)  from Brand Portal administrative tools.
Make sure that [separate Brand Portal tenants](#separate-tenants) are used for AEM Author instances configured with DM Hybrid and DM Scene7 modes, if you are using functionalities of DM Hybrid and DM S7.
* **Publish folders with video encodes applied to Brand Portal**
Apply [video encodings](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) and publish the folder containing rich media assets from AEM Author instance to Brand Portal.
* **Whitelist Egress IPs in SPS if secure preview enabled**
If using Dynamic Media-Scene 7 (with [secure preview enabled](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) for a company), then it is advised that Scene 7 company administrator [whitelists the public egress IPs](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) for respective regions using  SPS (Scene 7 Publishing System) flash UI.
The Egress IPs are as follows:

| **Region**  | **Egress IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

To whitelist either of these Egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Best Practices

To ensure that your dynamic video assets are successfully previewed, played, and downloaded from Brand Portal (and shared links), follow these practices:

### Separate tenants for Dynamic Media Hybrid and Dynamic Media Scene 7 modes {#separate-tenants}

If you are using both Dynamic Media Scene 7 and Dynamic Media Hybrid features, it is advised that you use different Brand Portal tenants for AEM Author instances configured with Dynamic Media Hybrid and Dynamic Media Scene 7 modes.
![Author and BP one to one mapping](assets/BPDynamicMedia.png)

### Same configuration details at AEM Author instance and Brand Portal

Ensure that the configuration details–such as Title, Registration ID, Video Service URL (in Dynamic Media Hybrid) and Title, credentials (Email and Password), Region, Company (in Dynamic Media Scene 7)–are the same in Brand Portal and AEM cloud configuration.

### Whitelist public egress IPs for Dynamic Media Scene 7 mode

If Dynamic Media Scene 7–having [secure preview enabled](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)–is used to serve video assets to Brand Portal, then Scene 7 establishes a dedicated Image Server for staging environments or internal applications. Any request to this server checks the origin IP address. If the incoming request is not within the approved list of IP addresses, a failure response is returned.
The Scene 7 Company Administrator, therefore, configures an approved list of IP addresses for their company’s Secure Testing environment, through SPS (Scene 7 Publishing System) flash UI. Make sure that the egress IP for your respective region (from the following) is added to that approved list.
To whitelist either of these Egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
The Egress IPs are as follows:

| **Region**  | **Egress IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configure Dynamic Media (Hybrid) settings {#configure-dm-hybrid-settings}

If AEM Author instance is running on dynamic media hybrid mode, then use Video tile from administrative tools panel to configure Dynamic Media gateway settings.
>[!NOTE]
>
>The [video encoding profiles](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) are not published to Brand Portal, instead are fetched from the Scene 7 server. Therefore, for video encodes to be played successfully in Brand Portal, ensure that the configuration details are the same as the [Scene7 cloud configuration](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in your AEM Author instance.
To set up Dynamic Media configurations on Brand Portal tenants:

1. Select the AEM logo to access administrative tools from the toolbar at the top, in Brand Portal.

2. From the administrative tools panel, select the **Video** tile.

![Dynamic Media Hybrid Config on Brand Portal](assets/DMHybrid-Video.png)

**Edit Dynamic Media Configuration** page opens.
![Dynamic Media Hybrid Configuration on Brand Portal](assets/edit-dynamic-media-config.png)

3. Specify **Registration ID** and **Video Service URL** (DM-Gateway URL). Make sure these details are the same as those in **Tools** > **Cloud Services** in your AEM Author instance.

4. Select **Save** to save the configuration.

## Configure Dynamic Media Scene7 settings {#configure-dm-scene7-settings}

If AEM Author instance is running on Dynamic Media- Scene 7 mode, then use **Dynamic Media Configuration** tile from administrative tools panel to configure the Scene 7 server settings.

To set up Dynamic Media Scene 7 configurations on Brand Portal tenants:

1. Select the AEM logo to access administrative tools from the toolbar at the top, in Brand Portal.

2. From the administrative tools panel, select the **Dynamic Media Configuration** tile.<br>
![DM Scene 7 configuration on Brand Portal](assets/DMS7-Tile.png)<br>
Edit Dynamic Media Configuration page opens.<br>
![Scene 7 Configuration on Brand Portal](assets/S7Config.png)

3. Provide:  
    * Title
    * Credentials (Email ID and Password) to access Scene 7 server
    * Region<br>
Make sure these values are the same as those in your AEM Author instance.

4. Select **Connect to Dynamic Media**.

5. Provide the **Company name**, and **Save** the configuration.
