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

Preview and play videos adaptively on [!DNL Brand Portal] with Dynamic Media support. Also download the dynamic renditions from the portal and shared links.
[!DNL Brand Portal] users can:

* Preview videos in Asset Details page, Card View, and link share preview page.
* Play video encodes on Asset Details page.
* View dynamic renditions in Renditions tab on Asset Details page.
* Download video encodes and folders containing videos.

>[!NOTE]
>
>To work with videos and to publish them to [!DNL Brand Portal], make sure that your [!DNL AEM] Author instance is set up either on Dynamic Media Hybrid mode or Dynamic Media [!DNL Scene 7] mode.

To preview, play, and download videos, [!DNL Brand Portal] exposes the following two configurations to administrators:

* [Dynamic Media Hybrid configuration](#configure-dm-hybrid-settings)
If [!DNL AEM] Author instance is running on dynamic media Hybrid mode.
* [Dynamic Media [!DNL Scene 7] configuration](#configure-dm-scene7-settings)
If [!DNL AEM] Author instance is running on dynamic media-[!DNL Scene 7] mode.
Set either of these configurations based on the configurations you set in your [!DNL AEM] Author instance with which [!DNL Brand Portal] tenant is replicated.

>[!NOTE]
>
>Dynamic videos are not supported on [!DNL Brand Portal] tenants integrated with [!DNL AEM] Author running on [!UICONTROL Scene7Connect] runmode.

## How are dynamic videos played? {#how-are-dynamic-videos-played}

![Video encodes are fetched from cloud](assets/VideoEncodes.png)

If Dynamic Media configurations ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) or [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configurations) are set up on [!DNL Brand Portal], the dynamic renditions are fetched from [!DNL Scene 7] server. Video encodes are, therefore, previewed and played without delay and distortion in quality.

As video encodes are not stored in [!DNL Brand Portal] repository and are fetched from [!DNL Scene 7] server, ensure that the Dynamic Media configurations on [!DNL AEM] Author Instance and [!DNL Brand Portal] are the same.

>[!NOTE]
>
>Video viewers and viewer presets are not supported in [!DNL Brand Portal]. Videos are previewed and played on the default viewers in [!DNL Brand Portal].

## Prerequisites {#prerequisites}

To work with dynamic videos on [!DNL Brand Portal], make sure to:

* **Start up [!DNL AEM] Author on DM (Dynamic Media) mode**
Start up the [!DNL AEM] Author instance (with which [!DNL Brand Portal] is integrated) either on [Dynamic Media Hybrid mode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) or [Dynamic Media [!DNL Scene 7] mode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configure Dynamic Media cloud services on [!DNL AEM] Author**
Based on the Dynamic Media mode [!DNL AEM] Author is running on, set either of [Dynamic Media cloud services](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) or [[!DNL Scene 7] cloud services](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) on [!DNL AEM] Author from **Tools** | **Cloud Services** | **Dynamic Media**.  
* **Configure Dynamic Media on Brand Portal**
Based on the Dynamic Media cloud configurations on [!DNL AEM] Author, configure [Dynamic Media settings](#configure-dm-hybrid-settings) or [[!DNL Scene 7] settings](#configure-dm-scene7-settings)  from [!DNL Brand Portal] administrative tools.
Make sure that [separate [!DNL Brand Portal] tenants](#separate-tenants) are used for [!DNL AEM] Author instances configured with Dynamic Media Hybrid and Dynamic Media [!UICONTROL Scene7] modes, if you are using functionalities of Dynamic Media Hybrid and Dynamic Media [!UICONTROL S7].
* **Publish folders with video encodes applied to Brand Portal**
Apply [video encodings](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) and publish the folder containing rich media assets from [!DNL AEM] Author instance to [!DNL Brand Portal].
* **Whitelist Egress IPs in SPS if secure preview enabled**
If using Dynamic Media-[!DNL Scene 7] (with [secure preview enabled](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) for a company), then it is advised that [!DNL Scene 7] company administrator [whitelists the public egress IPs](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) for respective regions using  SPS ([!UICONTROL Scene 7] Publishing System) flash UI.
The Egress IPs are as follows:

| **Region**  | **Egress IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

To whitelist either of these egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Best Practices

To ensure that your dynamic video assets are successfully previewed, played, and downloaded from [!DNL Brand Portal] (and shared links), follow these practices:

### Separate tenants for Dynamic Media Hybrid and Dynamic Media Scene 7 modes {#separate-tenants}

If you are using both Dynamic Media [!DNL Scene 7] and Dynamic Media Hybrid features, it is advised that you use different [!DNL Brand Portal] tenants for [!DNL AEM] Author instances configured with Dynamic Media Hybrid and Dynamic Media [!DNL Scene 7] modes.
![Author and BP one to one mapping](assets/BPDynamicMedia.png)

### Same configuration details at AEM Author instance and Brand Portal

Ensure that the configuration details–such as Title, Registration ID, Video Service URL (in Dynamic Media Hybrid) and Title, credentials (Email and Password), Region, Company (in Dynamic Media [!DNL Scene 7])–are the same in [!DNL Brand Portal] and [!DNL AEM] cloud configuration.

### Whitelist public egress IPs for Dynamic Media Scene 7 mode

If Dynamic Media Scene 7–having [secure preview enabled](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)–is used to serve video assets to [!DNL Brand Portal], then Scene 7 establishes a dedicated Image Server for staging environments or internal applications. Any request to this server checks the origin IP address. If the incoming request is not within the approved list of IP addresses, a failure response is returned.
The Scene-7 Company Administrator, therefore, configures an approved list of IP addresses for their company’s Secure Testing environment, through SPS (Scene-7 Publishing System) flash UI. Make sure that the egress IP for your respective region (from the following) is added to that approved list.
To whitelist either of these egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
The egress IPs are as follows:

| **Region**  | **Egress IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configure Dynamic Media (Hybrid) settings {#configure-dm-hybrid-settings}

If [!DNL AEM] Author instance is running on dynamic media hybrid mode, then use Video tile from administrative tools panel to configure Dynamic Media gateway settings.
>[!NOTE]
>
>The [video encoding profiles](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) are not published to [!DNL Brand Portal], instead are fetched from the Scene 7 server. Therefore, for video encodes to be played successfully in [!DNL Brand Portal], ensure that the configuration details are the same as the [Scene7 cloud configuration](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in your [!DNL AEM] Author instance.
To set up Dynamic Media configurations on [!DNL Brand Portal] tenants:

1. Select the [!DNL AEM] logo to access administrative tools from the toolbar at the top, in [!DNL Brand Portal].

2. From the administrative tools panel, select the **Video** tile.
![Dynamic Media Hybrid Config on Brand Portal](assets/DMHybrid-Video.png)
**Edit Dynamic Media Configuration** page opens.
![Dynamic Media Hybrid Configuration on Brand Portal](assets/edit-dynamic-media-config.png)

3. Specify **Registration ID** and **Video Service URL** (DM-Gateway URL). Make sure these details are the same as those in **Tools** > **Cloud Services** in your [!DNL AEM] Author instance.

4. Select **Save** to save the configuration.

## Configure Dynamic Media Scene7 settings {#configure-dm-scene7-settings}

If [!DNL AEM] Author instance is running on Dynamic Media- [!UICONTROL Scene 7] mode, then use **Dynamic Media Configuration** tile from administrative tools panel to configure the [!UICONTROL Scene 7] server settings.

To set up Dynamic Media [!UICONTROL Scene 7] configurations on [!DNL Brand Portal] tenants:

1. Select the [!DNL AEM] logo to access administrative tools from the toolbar at the top, in [!DNL Brand Portal].

2. From the administrative tools panel, select the **Dynamic Media Configuration** tile.
![DM Scene 7 configuration on [!DNL Brand Portal]](assets/DMS7-Tile.png)
Edit Dynamic Media Configuration page opens.
![Scene 7 Configuration on [!DNL Brand Portal]](assets/S7Config.png)

3. Provide:  
    * Title
    * Credentials (Email ID and Password) to access Scene 7 server
    * Region
Make sure these values are the same as those in your [!DNL AEM] Author instance.

4. Select **Connect to Dynamic Media**.

5. Provide the **Company name**, and **Save** the configuration.
