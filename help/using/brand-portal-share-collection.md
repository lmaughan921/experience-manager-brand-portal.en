---
title: Share a collection
seo-title: Share a collection
description: null
seo-description: AEM Assets Brand Portal Administrators can share and unshare a collection or a smart collection with authorized users. Editors can view and share only the collections created by them, shared with them, and public collections.
uuid: f70f811d-39a5-45dd-be81-4d10e95ec2c7
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 3da35f86-a5c2-44bf-86f7-3235bf853758
---

# Share a collection{#share-a-collection}

AEM Assets Brand Portal Administrators can share and un-share a collection or a smart collection with authorized users. Editors can view and share only the collections created by them, shared with them, and public collections. However, editors cannot change a public collection to a non-public collection.

>[!NOTE]
>
>Editors cannot change a public collection to a non-public collection and, therefore, do not have **Public Collection **check box available in** Collection Settings** dialog.

## Share a collection {#share-a-collection}

To share a collection, follow these steps:

1. Click the overlay icon on the left, and choose **Navigation**.

   ![](assets/ContentTree.png)

1. From the siderail on the left, click **Collections**.

   ![](assets/access_collections.png)

1. From the **Collections** console, do one of the following:

    * Hover the pointer over the collection you want to share. From the quick action thumbnails available for the collection, click the **Settings** icon.

   ![](assets/settings_thumbnail.png)

    * Select the collection you want to share. From the toolbar at the top, click **Settings**.

   ![](assets/collection-sharing.png)

1. In the **Collection Settings** dialog box, select the users or groups with whom you want to share the collection and select the role for a user or a group to match their global role. For example, assign the Editor role to a global editor, the Viewer role to a global viewer.

   Alternatively, to make the collection available to all users irrespective of their group membership and role, make it public by selecting the **Public Collection** check box.

   >[!NOTE]
   >
   >However, non-admin users can be restricted from creating public collections, to avoid having numerous public collections so that system space can be saved. Organizations can disable the **Allow public collections creation** configuration from **General** settings available in admin tools panel.

   ![](assets/collection_sharingadduser.png)

   Editors cannot change a public collection to a non-public collection and, therefore, do not have **Public Collection** check box available in **Collection Settings** dialog.

   ![](assets/Collection-Setting-Editor.png)

1. Click **Add**, and then **Save**. The collection is shared with the chosen users.

   >[!NOTE]
   >
   >A user's role governs access to the assets and folders inside a collection. If a user does not have access to assets, an empty collection is shared with the user. Also, a user's role governs the actions available for collections.

## Unshare a collection {#unshare-a-collection}

To unshare a previously shared collection, do the following:

1. From the **Collections** console, select the collection you want to unshare.

   In the toolbar, click **Settings**.

   ![](assets/collection_settings.png)

1. On the **Collection Settings** dialog box, under **Members**, click the **x** symbol next to users or groups to remove them from the list of users you shared the collection with.

   ![](assets/unshare_collection.png)

1. In the warning message box, click **Confirm** to confirm unshare.

   Click **Save**.

1. Log in to Brand Portal with the credentials of the user you removed from the shared list. The collection is removed from the **Collections** console.
