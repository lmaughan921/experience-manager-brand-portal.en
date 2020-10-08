---
title: Create Contribution folder
seo-title: Create Contribution folder
description: Get an insight on how to create a contribution folder in AEM Assets. 
seo-description: Get an insight on how to create a contribution folder in AEM Assets.
uuid: 
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 
---

# Create contribution folder {#create-contribution-folder}


AEM administrators and non-admin users having permission to create a new folder, can create a contribution folder in AEM Assets. 
To create a contribution folder, create a new folder of type Asset Contribution, ensuring the new folder created is open to asset submission by Brand Portal users.  This automatically triggers a workflow which creates two additional sub folders, called SHARED and NEW, within the contribution folder.

>[!NOTE]
>
>You can create multiple contribution folders within a folder but you must not not create a contribution folder inside another contribution folder.

To create a contribution folder:
1. Log in to your AEM author instance.

   The default URL is http:// localhost:4502/aem/start.html.

1. Navigate to **[!UICONTROL Assets]** > **[!UICONTROL Files]**. It lists all the existing folders in the AEM Assets repository.

1. Click **[!UICONTROL Create]** to create a new folder. **[!UICONTROL Create Folder]** dialog opens.

1. Enter **[!UICONTROL Title]** and **[!UICONTROL Name]** of the folder and select the **[!UICONTROL Asset Contribution]** check box.
It is recommended to use lowercase letters without any space to name the folder.

1. Click **[!UICONTROL Create]**. You can see the contribution folder listed in the AEM Assets repository.

   >[!NOTE]
   >
   >A non-admin user can create and share an asset contribution folder but cannot modify or delete it.  

   ![](assets/create-contribution-folder.png)

1. Click to open the contribution folder, you can see two sub folders–**[!UICONTROL SHARED]** and **[!UICONTROL NEW]** are automatically created within the contribution folder. 
  
   ![](assets/contribution-folder.png)

You can now [configure the contribution folder properties](brand-portal-configure-contribution-folder-properties.md). 


