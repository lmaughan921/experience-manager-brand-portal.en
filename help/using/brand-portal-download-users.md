---
title: Download assets
seo-title: Download assets
description: All users can simultaneously download multiple assets and folders accessible to them. This way, approved brand assets can be securely distributed for offline use.
seo-description: All users can simultaneously download multiple assets and folders accessible to them. This way, approved brand assets can be securely distributed for offline use.
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
index: y
internal: n
snippet: y
---

# Download assets{#download-assets}

All users can simultaneously download multiple assets and folders accessible to them from Brand Portal. This way, approved brand assets can be securely distributed for offline use. Read on to know how to download approved assets from Brand Portal, and what to expect from the [download performance](../using/brand-portal-download-users.md#main-pars-header).

>[!NOTE]
>
>Only Administrators can download expired assets. For more information about expired assets, see [Manage digital rights of assets](../using/manage-digital-rights-of-assets.md).

## Steps to download assets {#steps-to-download-assets}

To download assets or folders containing assets for Brand Portal, follow these steps:

1. From the Brand Portal interface, do one of the following:

    * Select the folders or assets you want to download. From the toolbar at the top, click the **Download** icon.

   ![](assets/downloadassets-1.png)

    * To download a single folder or an asset, hover the pointer over the folder or the asset. From the quick action thumbnails available, click the **Download** icon.

   ![](assets/downloadsingleasset-1.png)

   >[!NOTE]
   >
   >If the assets you are downloading also include licensed assets, you are redirected to the **Copyright Management** page. In this page, select the assets, click **Agree**, and then click **Download**. If you choose to disagree, licensed assets are not downloaded.  
   >License-protected assets have [license agreement attached](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) to them, which is done by setting asset's [metadata property](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in AEM Assets.

   ![](assets/licensed-asset-download-1.png)

   The **Download** dialog box appears with the **Asset(s) **option selected by default.

   ![](assets/donload-assets-dialog-1.png)

   >[!NOTE]
   >
   >If the assets you are downloading are image files, and you select only the **Asset(s)** option in Download dialog but are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) then no image files are downloaded and a Notice prompts, stating that you have been restricted by administrator to access original renditions.

   ![](assets/restrictaccess-note.png)

1. To download the renditions of assets in addition to the assets, select **Rendition(s)**. However, to allow auto-generated renditions to download along with custom renditions, deselect **Exclude Auto Generated Renditions**, which is selected by default.

   ![](assets/exclude-auto-renditions.png)

   To download only the renditions, deselect **Asset(s)**.

   >[!NOTE]
   >
   >By default, only the assets are downloaded. However, original renditions of image files are not downloaded if you are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

    * To speed up the download of asset files from Brand Portal, select **Enable download acceleration **option and [follow the wizard](../using/accelerated-download.md#main-pars-header-405749062). To know more about faster download of assets refer [Guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).

    * To apply a [custom image preset to the asset and its renditions](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), select **Dynamic Rendition(s)**. Specify custom image preset properties (size, format, color space, resolution, and image modifier) to apply the custom image preset while downloading the asset and its renditions. To download only the dynamic renditions, delesect **Asset(s)**.

   ![](assets/dynamic-renditions.png)

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
   >Administrators can customize email messages, that is, logo, description, and footer, using the [Branding](../using/brand-portal-branding.md) feature.

1. Click **Download**.

   The assets (and renditions if selected) are downloaded as a ZIP file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions, thereby ensuring speedy download.

   Original renditions of the selected assets are not downloaded if you are not [authorized by administrator to have access to the original renditions](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   >[!NOTE]
   >
   >Assets that are selected individually and downloaded are visible in the assets downloaded report. However, if a folder containing assets is downloaded, neither the folder nor the assets are displayed in the assets downloaded report.

   To know how to download assets from shared links, refer [downloading assets from shared links](../using/brand-portal-link-share.md#main-pars-header-1703469193).

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
