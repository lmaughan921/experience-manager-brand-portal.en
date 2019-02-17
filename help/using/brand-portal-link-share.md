---
title: Share assets as a link
seo-title: Share assets as a link
description: AEM Assets Brand Portal Administrators can share links of multiple assets with authorized internal users and external entities, including partners and vendors. Editors can view and share only the assets shared with them.
seo-description: AEM Assets Brand Portal Administrators can share links of multiple assets with authorized internal users and external entities, including partners and vendors. Editors can view and share only the assets shared with them.
uuid: 8889ac24-c56d-4a47-b792-80c34ffb5c3f
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
index: y
internal: n
snippet: y
---

# Share assets as a link{#share-assets-as-a-link}

AEM Assets Brand Portal Administrators can share links of multiple assets with authorized internal users and external entities, including partners and vendors. Editors can view and share only the assets shared with them.

Sharing assets through a link is a convenient way of making them available to external parties as the receivers do not have to log in to Brand Portal to access the assets.

Link sharing access is restricted to editors and administrators. For more information, see [Managing users, groups, and user roles](../using/brand-portal-adding-users.md).

>[!NOTE]
>
>Upto 5GB of zip download is allowed using link share feature on brand portal.

## Share assets as a link {#share-assets-as-a-link}

To share assets as a link, follow these steps:

1. Click the overlay icon on the left, and choose **Navigation**.

   ![](assets/siderail.png)

1. From the siderail on the left, click **Files** to share folders or images. To share collections, click **Collections**. 

   ![](assets/navigationrail.png)

1. Select the folders or collections you want to share as a link.

   ![](assets/asset-link-share.png)

1. From the toolbar at the top, click the **Share Link** icon.

   The **Link Sharing** dialog box appears.

   ![](assets/link-sharing.png)

   >[!NOTE]
   >
   >The **Share Link** field displays an automatically created asset link. The default expiry time for this link is 7 days. You can copy the link and share it separately with users or share it from the **Link Sharing** dialog box.

1. In the email address box, type the email ID of the user with whom you want to share the link. You can share the link with multiple users.

   If the user is a member of your organization, select their email ID from the suggestions that appear in the drop-down list. If the user is external, type the complete email ID and press **Enter**; the email ID is added to the list of users.

   ![](assets/link-sharing-text.png)

1. In the **Subject** box, type a subject for the asset you want to share.
1. In the **Message** box, type a message if necessary.
1. In the **Expiration** field, use the date picker to specify an expiration date and time for the link. By default, the expiry date is set to 7 days from the date on which you share the link.

   The assets shared through the link expire after crossing the date and time specified in the **Expiration** field. For information about the behavior of expired assets and changes in the permissible activities based on user roles in Brand Portal, see [Manage digital rights of assets](../using/manage-digital-rights-of-assets.md).

1. Click **Share**. A message confirms that the link is shared with the users. Users receive an email containing the link.

   ![](assets/link-sharing-email.png)

   >[!NOTE]
   >
   >Administrators can customize the email messaging, that is, logo, description, and footer, using the [Branding](../using/brand-portal-branding.md#customizetheemailmessaging) feature.

## Download assets from shared links {#download-assets-from-shared-links}

Click the link in the email, to view the shared asset. The AEM Link Share page opens.

To download the shared assets:

1. Click the assets and then click **Download **icon from the toolbar.

   ![](assets/assets-shared-link.png)

   >[!NOTE]
   >
   >Currently, you can generate a preview and thumbnail only for certain assets, depending on the file format. For more information about the supported file formats, see [Preview and thumbnail support for asset formats](#preview-thumbnail-support).

   >[!NOTE]
   >
   >If the assets you are downloading also include licensed assets, you are redirected to the **Copyright Management** page. In this page, select the licensed assets, click **Agree**, and then click **Download**. If you choose to disagree, only the unlicensed assets are downloaded.  
   >License-protected assets have [license agreement attached](/content/help/en/experience-manager/6-4/assets/using/drm#main-pars_text) to them, which is done by setting asset's [metadata property](/content/help/en/experience-manager/6-4/assets/using/drm#main-pars_text) in AEM Assets.

   ![](assets/licensed-asset-download.png)

   The **Download **dialog box appears. 

   ![](assets/download-linkshare.png)

    * To speed up the download of asset files shared as the link, select **Enable download acceleration **option and [follow the wizard](../using/accelerated-download.md#main-pars-header-405749062). To know more about the fast download of assets on Brand Portal refer [Guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).

1. To download the renditions of assets in addition to the assets from the shared link, select **Rendition(s) **option. When you do so,** Exclude System Renditions **option appears that is selected by default. This prevents the download of out-of-the-box renditions along with approved assets or their custom renditions.

   However, to allow auto-generated renditions to download along with custom renditions, deselect the **Exclude System Renditions** option.

   >[!NOTE]
   >
   >Original renditions are not downloaded using the shared link if the user who shared the assets as a link is not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   ![](assets/download-linkshare-autoren.png)

1. Tap/ click **Download**. The assets (and renditions if selected) are downloaded as a ZIP file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions, thereby ensuring speedy download.

>[!NOTE]
>
>Brand Portal restricts downloading assets larger than 5 GB per file size.

## Preview and thumbnail support for asset formats {#preview-thumbnail-support}

The following matrix lists the asset formats for which Brand Portal supports thumbnail and preview:

<table border="1" cellpadding="1" cellspacing="0" width="100%"> 
 <tbody> 
  <tr> 
   <td>Asset format</td> 
   <td>Thumbnail support</td> 
   <td>Preview support</td> 
  </tr> 
  <tr> 
   <td>PNG</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>GIF</td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>TIFF</td> 
   <td>✓ </td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>JPEG</td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>BMP </td> 
   <td>✓ </td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>PNM*</td> 
   <td>NA</td> 
   <td>NA<br /> </td> 
  </tr> 
  <tr> 
   <td>PGM*</td> 
   <td>NA<br /> </td> 
   <td>NA<br /> </td> 
  </tr> 
  <tr> 
   <td>PBM*</td> 
   <td>NA<br /> </td> 
   <td>NA<br /> </td> 
  </tr> 
  <tr> 
   <td>PPM*</td> 
   <td>NA<br /> </td> 
   <td>NA<br /> </td> 
  </tr> 
  <tr> 
   <td>PSD <br /> </td> 
   <td>✓ </td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>EPS</td> 
   <td>NA<br /> </td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>DNG </td> 
   <td>✓</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>PICT</td> 
   <td>✓</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>PSB*</td> 
   <td>✓</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>JPG </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>AI </td> 
   <td>✓</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>DOC</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>DOCX</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>ODT*</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>PDF </td> 
   <td>✓</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>HTML</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>RTF</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>TXT </td> 
   <td>✓</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>XLS</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>XLSX</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>ODS</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>PPT </td> 
   <td>✓</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>PPTX</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>ODP</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>INDD </td> 
   <td>✓</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>PS</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>QXP</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>EPUB</td> 
   <td>✓</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>AAC</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>MIDI</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>3GP</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>MP3</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>MP4 </td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>OGA</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>OGG</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>RA</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>WAV</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>WMA</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>DVI</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>FLV</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>M4V</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>MPG</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>OGV</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>MOV</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>WMV</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>SWF</td> 
   <td>✕</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>TGZ</td> 
   <td>NA<br /> </td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>JAR</td> 
   <td>✓</td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>RAR</td> 
   <td>NA<br /> </td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>TAR</td> 
   <td>NA<br /> </td> 
   <td>✕</td> 
  </tr> 
  <tr> 
   <td>ZIP</td> 
   <td>✓</td> 
   <td>✕</td> 
  </tr> 
 </tbody> 
</table>

The following legend explains the symbols used in the matrix:

| Symbol |Meaning |
|---|---|
| ✓ |This file format supports this feature  |
| ✕ |This file format does not support this feature  |
| NA |This feature is not applicable to this file format |
| &#42; |This feature requires add-on support for this file format on AEM author instance but not on Brand Portal after assets are published to Brand Portal |

## Unshare assets shared as a link {#unshare-assets-shared-as-a-link}

To unshare previously shared assets as a link, do the following:

1. To view the assets you shared as links, click the overlay icon on the left, and choose **Navigation**.

   ![](assets/siderail.png)

1. From the siderail, click **Shared Links**.

   ![](assets/navigationrail.png)

1. Review the links you shared from the list displayed.
1. To unshare a link from the list, select it and click the bin icon next to the link entry, or the **Unshare** icon from the toolbar at the top.

   ![](assets/unshare-links.jpg)

   >[!NOTE]
   >
   >The display of shared links is user-specific. This feature does not display all the links shared by all users of a tenant.

1. In the warning message box, click **Continue** to confirm unshare. The entry for the link is removed from the list of shared links.

