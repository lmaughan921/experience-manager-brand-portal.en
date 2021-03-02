---
title: Upload assets and publish the Contribution folder from Brand Portal to AEM Assets
seo-title: Upload assets and publish the Contribution folder from Brand Portal to AEM Assets
description: Get an insight into uploading new assets and publishing the contribution folder from Brand Portal to AEM Assets.
seo-description: Get an insight into uploading new assets and publishing the contribution folder from Brand Portal to AEM Assets.
uuid: 
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 
---

# Publish contribution folder assets from Brand Portal to AEM Assets {#using-asset-souring-in-bp}

Brand Portal users with appropriate permissions can upload multiple assets, or folders containing multiple assets, to the contribution folder. However, Brand Portal users are only able to upload assets to the **NEW** folder. The **SHARED** folder is meant for the distribution of baseline assets (reference content) which can be used by the Brand Portal users while creating new assets for contribution.

Brand Portal user having permission to access the contribution folder can perform the following activities:

* [Download asset requirements](#download-asset-requirements)
* [Upload new assets to the contribution folder](#uplad-new-assets-to-contribution-folder)
* [Publish contribution folder to AEM Assets](#publish-contribution-folder-to-aem)

## Download asset requirements {#download-asset-requirements}

Brand Portal users automatically receive email/pulse notifications whenever a contribution folder is shared by the AEM user, allowing them to download the brief (asset requirement) document, as well as download the baseline assets (reference content), from the **SHARED** folder to ensure they understand the asset requirements.

Brand Portal user performs the following activities to download asset requirements:

* **Download brief**: Download the brief (asset requirement document) attached to the contribution folder which contains asset related information like type of assets, purpose, supported formats, maximum asset size, etc.
* **Download baseline assets**: Download the baseline assets which can be used to understand the types of assets required. Brand Portal users can use these assets as reference to create new assets for contribution.

Brand Portal dashboard reflects all the existing folders permitted to the Brand Portal user along with the newly shared contribution folder. In this example, the Brand Portal user only has access to the newly created contribution folder, no other existing folder is shared with the user.

**To download asset requirements:**

1. Log in to your Brand Portal instance.
1. Select contribution folder from the Brand Portal dashboard.
1. Click **[!UICONTROL Properties]** ![](assets/properties.png). Property window opens, displaying the Asset Contribution folder details.
![](assets/download-asset-requirement1.png)
1. Click **[!UICONTROL Download Brief]** ![](assets/download.png) to download the asset requirement document on your local machine.
![](assets/download-asset-requirement2.png)
1. Go back to the Brand Portal dashboard.
1. Click to open the contribution folder, you can see two sub folders–**[!UICONTROL SHARED]** and **[!UICONTROL NEW]** within the contribution folder. The SHARED folder contains all the baseline assets (reference content) shared by the administrators. 
1. You can download the **[!UICONTROL SHARED]** folder containing all the baseline assets on your local machine. 
Or, you can to open the **[!UICONTROL SHARED]** folder and click **Download** icon ![](assets/download.png) to download individual files/folders.
![](assets/download-asset-requirement3.png)

Go through the brief (asset requirement document) and refer to the baseline assets to understand the asset requirements. Now, you can create new assets for contribution and upload them to the contribution folder. See, [Upload assets to contribution folder](brand-portal-upload-assets-to-contribution-folder.md).


## Upload assets to contribution folder {#uplad-new-assets-to-contribution-folder}

After going through the asset requirements, the Brand Portal users can create new assets for contribution and upload them to the NEW folder within the contribution folder.

>[!NOTE]
>
>The Brand Portal users can upload assets only to the NEW folder.
>
>The maximum upload limit for any Brand Portal tenant is **10**GB which is cumulatively applied to all the contribution folders. 

>[!NOTE]
>
>It is recommended to release the upload space after publishing the contribution folder to AEM Assets so that it is available to the other Brand Portal users for contribution. 
>
>If there is a need to extend the upload limit of your Brand Portal tenant beyond **10**GB, contact Adobe Support specifying the requirement.


**To upload new assets:**

1. Log in to your Brand Portal instance.
The Brand Portal dashboard reflects all the existing folders permitted to the Brand Portal user along with the newly shared contribution folder.

1. Select the contribution folder and click to open it. The contribution folder contains two sub folders – **[!UICONTROL SHARED]** and **[!UICONTROL NEW]**.

1. Click on the **[!UICONTROL NEW]** folder.

   ![](assets/upload-new-assets1.png)

1. Click **[!UICONTROL Create]** > **[!UICONTROL Files]** to upload individual files or folder (.zip) containing multiple assets.

   ![](assets/upload-new-assets2.png)

1. Browse and upload assets (files or folders) to the **[!UICONTROL NEW]** folder.

   ![](assets/upload-new-assets3.png)

After uploading all the assets or folders to the NEW folder, publish the contribution folder to AEM Assets. See, [Publish contribution folder to AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md).


## Publish contribution folder to AEM Assets {#publish-contribution-folder-to-aem}

Brand Portal users can publish the contribution folder to AEM Assets without needing access to the AEM author instance.

Ensure that you have gone through the [asset requirements](brand-portal-download-asset-requirements.md) and upload the newly created assets in **NEW** folder within the contribution folder. See, [Upload assets to contribution folder](brand-portal-upload-assets-to-contribution-folder.md). 

**To publish contribution folder:**

1. Log in to your Brand Portal instance.

1. Select contribution folder from the Brand Portal dashboard.
1. Click **[!UICONTROL Publish to AEM]**. 

   ![](assets/export.png)
   
   ![](assets/publish-contribution-folder-to-aem.png)

An email/pulse notification is sent to the Brand Portal user and administrators at different stages of the publishing workflow:
1. **Queued** - A notification is sent to the Brand Portal user and Brand Portal administrators when a publishing workflow triggers in Brand Portal.

1. **Complete** - A notification is sent to the Brand Portal user and Brand Portal administrators when the contribution folder is successfully published to AEM Assets.

After publishing the newly created assets to AEM Assets, the Brand Portal users can delete them from the NEW folder. Whereas, the Brand Portal administrator can delete the assets from both NEW and SHARED folder. 

Once the objective of creating the contribution folder is achieved, the Brand Portal administrator can delete the contribution folder to release the upload space for other users. 

**Publishing job status**

There are two reports which the administrators can utilize to view the status of the asset contribution folders published from Brand Portal to AEM Assets. 

* In Brand Portal, navigate to **[!UICONTROL Tools]** > **[!UICONTROL Asset Contribution Status]**. This report reflects the status of all the publishing jobs at different stages of the publishing workflow.  

  ![](assets/contribution-folder-status.png)

* In AEM Assets author instance, navigate to **[!UICONTROL Tools]** > **[!UICONTROL Jobs]**. This report reflects the final state (Success or Error) of all the publishing jobs. 

  ![](assets/publishing-status.png)

>[!NOTE]
>
>The user interface of AEM Assets as a Cloud Service is slightly different then the Managed Services or On-premises AEM Assets instance.






