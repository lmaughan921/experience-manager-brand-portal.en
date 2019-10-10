---
title: Upload Brand Portal users list
seo-title: Upload Brand Portal users list
description: Get an insight on how to upload Brand Portal user list in AEM Assets. 
seo-description: Get an insight on how to upload Brand Portal user list in AEM Assets.
uuid: 
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 
---

# Upload Brand Portal users list {#upload-bp-user-list}

AEM administrators can upload the Brand Portal user configuration (.csv) file containing active Brand Portal user list in AEM Assets. A contribution folder can only be shared with the active Brand Portal users defined in the user list. Administrator can also add new users in the configuration file and upload the modified user list.

Administrator can add new users in AEM Admin Console, see [Manage Users](brand-portal-adding-users.md) for detailed information. After adding users in Admin Console, these users can be added to the Brand Portal user configuration file and then assigned permission to access the contribution folder.

**To upload Brand Portal users list:**
1. Login to your AEM author instance
Default URL: http:// localhost:4502/aem/start.html
1. From **Tools** ![](assets/tools.png) panel, navigate to **[!UICONTROL Assets > Brand Portal Users]**
![](assets/upload-user-list1.png)
1. Brand Portal Upload Contributors window opens.
Browse from your local machine and upload **configuration (.csv) file** containing the active Brand Portal users list.
1. Click **[!UICONTROL Save]**.
![](assets/upload-user-list2.png)


Administrators can provide access to specific users/groups from this user list while configuring the contribution folder.

For more information, see [Configure contribution folder](brand-portal-contribution-folder.md).
