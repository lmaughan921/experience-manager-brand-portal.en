---
title: Download assets
seo-title: Download assets
description: null
seo-description: All users can simultaneously download multiple assets and folders accessible to them. This way, approved brand assets can be securely distributed for offline use.
uuid: bbf96647-5930-44aa-86dd-b266ac8d993f
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: cc4661b8-efe2-426f-b72d-1fe5d3165e89
isreadyforlocalization: false
index: y
internal: n
snippet: y
---

# Download assets{#download-assets}

All users can simultaneously download multiple assets and folders accessible to them from Brand Portal. This way, approved brand assets can be securely distributed for offline use. Read on to know how to download approved assets from Brand Portal, and what to expect from the [download performance](/brand-portal-download-users.md#main-pars_header).

>[!NOTE]
>
>Only Administrators can download expired assets. For more information about expired assets, see [Manage digital rights of assets](/manage-digital-rights-of-assets.md).

## Steps to download assets {#steps-to-download-assets}

To download assets or folders containing assets for Brand Portal, follow these steps:

1. From the Brand Portal interface, do one of the following:

    * Select the folders or assets you want to download. From the toolbar at the top, click the **Download** icon.

   ![](assets/DownloadAssets.png)

    * To download a single folder or an asset, hover the pointer over the folder or the asset. From the quick action thumbnails available, click the **Download** icon.

   ![](assets/DownloadSingleAsset.png)

   >[!NOTE]
   >
   >If the assets you are downloading also include licensed assets, you are redirected to the **Copyright Management** page. In this page, select the assets, click **Agree**, and then click **Download**. If you choose to disagree, licensed assets are not downloaded.  
   >License-protected assets have [license agreement attached](/content/help/en/experience-manager/6-4/assets/using/drm#main-pars_text) to them, which is done by setting asset's [metadata property](/content/help/en/experience-manager/6-4/assets/using/drm#main-pars_text) in AEM Assets.

   ![](assets/Licensed-Asset-download.png)

   The **Download** dialog box appears with the **Asset(s) **option selected by default.

   ![](assets/Donload-Assets-Dialog.png)

   >[!NOTE]
   >
   >If the assets you are downloading are image files, and you select only the **Asset(s)** option in Download dialog but are not [authorized by the administrator to have access to the original renditions of image files](/brand-portal-adding-users.md#main-pars_procedure_202029708) then no image files are downloaded and a Notice prompts, stating that you have been restricted by administrator to access original renditions.

   ![](assets/RestrictAccess-Note.png)

1. To download the renditions of assets in addition to the assets, select **Rendition(s)**. However, to allow auto-generated renditions to download along with custom renditions, deselect **Exclude Auto Generated Renditions**, which is selected by default.

   ![](assets/Exclude-Auto-Renditions.png)

   To download only the renditions, deselect **Asset(s)**.

   >[!NOTE]
   >
   >By default, only the assets are downloaded. However, original renditions of image files are not downloaded if you are not [authorized by the administrator to have access to the original renditions of image files](/brand-portal-adding-users.md#main-pars_procedure_202029708).

    * To speed up the download of asset files from Brand Portal, select **Enable download acceleration **option and [follow the wizard](/accelerated-download.md#main-pars_header_405749062). To know more about faster download of assets refer [Guide to accelerate downloads from Brand Portal](/accelerated-download.md).

    * To apply a [custom image preset to the asset and its renditions](/brand-portal-image-presets.md#Applyimagepresetswhendownloadingimages), select **Dynamic Rendition(s)**. Specify custom image preset properties (size, format, color space, resolution, and image modifier) to apply the custom image preset while downloading the asset and its renditions. To download only the dynamic renditions, delesect **Asset(s)**.

   ![](assets/Dynamic-Renditions.png)

   >[!NOTE]
   >
   >To be able to preview (or download) dynamic renditions of any asset, ensure that the dynamic media is enabled and the asset's PTIFF rendition exists at the AEM author instance, from where the assets have been published. When an asset is published to Brand Portal, its PTIFF rendition is also published. There is no way of generating the PTIFF rendition from Brand Portal.

    * To preserve the Brand Portal folder hierarchy while downloading assets, select **Create separate folder for each asset**. By default, Brand Portal folder hierarchy is ignored and all assets are downloaded in one folder in your local system.

    * To send an email notification to users with a link for downloading the assets, select **Email**.

   ![](assets/download-link.png)

   >[!NOTE]
   >
   >Download link on email notification expires after 45 days.
   >
   >
   >Administrators can customize email messages, that is, logo, description, and footer, using the [Branding](/brand-portal-branding.md) feature.

1. Click **Download**.

   The assets (and renditions if selected) are downloaded as a ZIP file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions, thereby ensuring speedy download.

   Original renditions of the selected assets are not downloaded if you are not [authorized by administrator to have access to the original renditions](/brand-portal-adding-users.md#main-pars_procedure_202029708).

   >[!NOTE]
   >
   >Assets that are selected individually and downloaded are visible in the assets downloaded report. However, if a folder containing assets is downloaded, neither the folder nor the assets are displayed in the assets downloaded report.

   To know how to download assets from shared links, refer [downloading assets from shared links](/brand-portal-link-share.md#main-pars_header_1703469193).

## Expected download performance {#expected-download-performance}

File download experience may vary for users at different client locations, depending on factors such as local Internet connectivity and server latency. The expected download performance for 2 GB file observed at different client locations is as follows, with Brand Portal server at Oregon in United States:

<table border="1" cellpadding="0" cellspacing="0" width="661"> 
 <tbody>
  <tr>
   <td valign="top" width="156"><p><strong>Client location</strong></p> </td> 
   <td valign="top" width="103"><p><strong>Latency between client and server</strong></p> </td> 
   <td valign="top" width="129"><p><strong>Expected download speed</strong></p> </td> 
   <td valign="top" width="156"><p><strong>Time 
      <g class="gr_ gr_71 gr-alert gr_gramm gr_inline_cards gr_disable_anim_appear Grammar multiReplace" data-gr-id="71" id="71">
       taken
      </g> to download a 2 GB file</strong></p> </td> 
  </tr>
  <tr>
   <td valign="top" width="156"><p>US West (N. California)</p> </td> 
   <td valign="top" width="103"><p>18 milliseconds</p> </td> 
   <td valign="top" width="129"><p>7.68 MB/s</p> </td> 
   <td valign="top" width="156"><p>4 minutes</p> </td> 
  </tr>
  <tr>
   <td valign="top" width="156"><p>US West (Oregon)</p> </td> 
   <td valign="top" width="103"><p>42 milliseconds</p> </td> 
   <td valign="top" width="129"><p>3.84 MB/s</p> </td> 
   <td valign="top" width="156"><p>9 minutes</p> </td> 
  </tr>
  <tr>
   <td valign="top" width="156"><p>US East (N. Virginia)</p> </td> 
   <td valign="top" width="103"><p>85 milliseconds</p> </td> 
   <td valign="top" width="129"><p>1.61 MB/s</p> </td> 
   <td valign="top" width="156"><p>21 minutes</p> </td> 
  </tr>
  <tr>
   <td valign="top" width="156"><p>APAC (Tokyo)</p> </td> 
   <td valign="top" width="103"><p>124 milliseconds</p> </td> 
   <td valign="top" width="129"><p>1.13 MB/s</p> </td> 
   <td valign="top" width="156"><p>30 minutes</p> </td> 
  </tr>
  <tr>
   <td valign="top" width="156"><p>Noida</p> </td> 
   <td valign="top" width="103"><p>275 milliseconds</p> </td> 
   <td valign="top" width="129"><p>0.5 MB/s</p> </td> 
   <td valign="top" width="156">68 minutes</td> 
  </tr>
  <tr>
   <td valign="top" width="156"><p>Sydney</p> </td> 
   <td valign="top" width="103"><p>175 milliseconds</p> </td> 
   <td valign="top" width="129"><p>0.49 MB/s</p> </td> 
   <td valign="top" width="156"><p>69 minutes</p> </td> 
  </tr>
  <tr>
   <td valign="top" width="156"><p>London</p> </td> 
   <td valign="top" width="103"><p>179 milliseconds</p> </td> 
   <td valign="top" width="129"><p>0.32 MB/s</p> </td> 
   <td valign="top" width="156"><p>106 minutes</p> </td> 
  </tr>
  <tr>
   <td valign="top" width="156"><p>Singapore</p> </td> 
   <td valign="top" width="103"><p>196 milliseconds</p> </td> 
   <td valign="top" width="129"><p>0.5 MB/s<br /> </p> </td> 
   <td valign="top" width="156">68 minutes</td> 
  </tr>
 </tbody>
</table>

**Note**: Cited data are observed under test conditions, which may vary for users at different locations witnessing varied latency and bandwidth.
