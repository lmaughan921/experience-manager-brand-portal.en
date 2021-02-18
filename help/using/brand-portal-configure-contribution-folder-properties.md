---
title: Configure Contribution folder properties
seo-title: Configure Contribution folder properties
description: Get an insight on how to configure the properties of a contribution folder in AEM Assets. 
seo-description: Get an insight on how to configure the properties of a contribution folder in AEM Assets. 
uuid: 
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
version: 6.5
discoiquuid: 
---

# Configure contribution folder properties {#configure-contribution-folder-properties}

AEM administrator performs the following activities while configuring the properties of a contribution folder.

* **Add description**: Provide a high-level description of the contribution folder.
* **Upload brief**:  Upload Asset Requirement document containing asset related information.
* **Add contributors**: Add Brand Portal users to grant them access to the contribution folder.

Asset requirement refers to the details provided by administrators to help contributors (Brand Portal users) understand the need and requirements of the contribution folder. Administrator uploads an asset requirement document which contains a brief about the type of assets that should be added to the contribution folder and asset related information, for example, purpose, type of images, max size, etc.

**To configure contribution folder properties:**

1. Log in to your AEM author instance
Default URL: http:// localhost:4502/aem/start.html
1. Navigate to **[!UICONTROL Assets > Files]** and locate the contribution folder.
1. Select contribution folder and click **[!UICONTROL Properties]** to open the Folder properties window.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. Navigate to **[!UICONTROL Asset Contribution]** tab.
1. Enter high-level **[!UICONTROL Description]** of the contribution folder.
1. Click **[!UICONTROL Upload Brief]** to browse from your local machine and upload an **Asset Requirement Document**.

   ![](assets/upload.png) 

1. In the **[!UICONTROL Add User]** field, add Brand Portal users with whom you want to share the contribution folder. These users can access and upload content to the contribution folder using the Brand Portal interface.
1. Click **[!UICONTROL Save]**.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>Currently, groups cannot be assigned to a contribution folder.
>
>The search results are based on the Brand Portal user list configured in AEM Assets. Make sure you have the updated Brand Portal user list. See, [Upload Brand Portal user list](brand-portal-configure-asset-sourcing.md).
