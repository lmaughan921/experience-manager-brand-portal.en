---
title: Manage groups
seo-title: Manage groups
description: A group in AEM Assets Brand Portal is the same as a product profile in Adobe Admin Console. Administrators use Adobe Admin Console to create a product profile, which is then synced with the Brand Portal user interface and visible as a group in Brand Portal. 
seo-description: A group in AEM Assets Brand Portal is the same as a product profile in Adobe Admin Console. Administrators use Adobe Admin Console to create a product profile, which is then synced to Brand Portal as a group. Administrators can then add users to the group. The user-to-group association, or the group membership of a user, in Adobe Admin Console, is synced with Brand Portal every 8 hours. Changes to user or group roles are effective in Brand Portal after the next sync job runs. However, to manage group roles, Administrators must use the Brand Portal user interface. This privilege is not available to Viewers and Editors.
page-status-flag: never-activated
uuid: 47a40e57-af84-4ecd-85df-042198b9fca8
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 812b7600-c575-4b50-8457-9c98535fe182
index: y
internal: n
snippet: y
---

# Manage groups{#manage-groups}

A group in AEM Assets Brand Portal is the same as a product profile in Adobe Admin Console. Administrators use Adobe Admin Console to create a product profile, which is then synced with the Brand Portal user interface and visible as a group in Brand Portal. 

Administrators can then use Admin Console to add users to the product profile. The user-to-group association, or the group membership of a user in Adobe Admin Console, is synced with Brand Portal every 8 hours. Changes to user or group roles are effective in Brand Portal after the next sync job runs.

## Log in to Adobe Admin Console {#log-in-to-adobe-admin-console}

You can login to Admin Console directly, through the URL https://adminconsole.adobe.com/enterprise/overview, or from Brand Portal. Follow the procedure below to login to Admin Console from Brand Portal.

1. From the AEM toolbar at the top, click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

1. From the administrative tools panel, click **Users**.

   ![](assets/Admin-tools-panel-3.png)

1. In the **User Roles** page, click the **Management** tab, then click **Launch Admin Console**.

   ![](assets/launch_admin_console.png)

## Create a group {#create-a-group}

In [Admin Console](https://adminconsole.adobe.com/enterprise/overview), you can view all Adobe products associated with your organization. A product could be any Experience Cloud solution, such as Adobe Analytics, Adobe Target, or AEM Brand Portal. Brand Portal administrators must choose the AEM Brand Portal product and create groups.

Product profiles in Admin Console are used to create groups in Brand Portal so that you can perform bulk operations such as role management and asset sharing in Brand Portal. **Assets Brand Portal** is the default product profile available; you can create more product profiles and add users to the new product profiles.

>[!NOTE]
>
>To create groups in Brand Portal, from Adobe Admin Console, use **Products** page &gt; **Product Profiles**, instead of **User** page &gt; **User Groups**.

1. Log in to Admin Console directly, through the URL [https://adminconsole.adobe.com/enterprise/overview](https://adminconsole.adobe.com/enterprise/overview), or from Brand Portal. For the steps to log in from Brand Portal, see [Log  in to  Adobe Admin Console](/brand-portal-manage-groups.md#LogintoAdobeAdminConsole).
1. From the toolbar at the top, click **Products**. 
1. In the **Products** page, **Product Profiles** is selected by default. Click **New Profile**. 

   ![](assets/admin_console_addproductprofile.png)

1. In the **Create a New Profile** page, provide the profile name, display name, profile description, and choose if you want to notify users by email when they are added to or removed from the profile.

   ![](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. Click **Done**. The product configuration group, for example **Sales group**, is added to Brand Portal.

   ![](assets/admin_console_productprofileadded.png)

## Delete a group {#delete-a-group}

Brand Portal administrators can delete existing groups in the AEM Brand Portal product.

1. Log in to Admin Console directly, through the URL [https://adminconsole.adobe.com/enterprise/overview](https://adminconsole.adobe.com/enterprise/overview), or from Brand Portal. For the steps to log in from Brand Portal, see [Log  in to  Adobe Admin Console](/brand-portal-manage-groups.md#LogintoAdobeAdminConsole).
1. In the **Product Details** page, select the check boxes to the left of the product profile name and click **Delete Profile**.
1. In the confirmation dialog box, click **Delete Profile**.

## Add users to a group {#add-users-to-a-group}

To add users to a Brand Portal group, add them to the corresponding product profile in Admin Console. You can add users individually or in bulk.

1. Log in to Admin Console directly, through the URL [https://adminconsole.adobe.com/enterprise/overview](https://adminconsole.adobe.com/enterprise/overview), or from Brand Portal. For the steps to log in from Brand Portal, see [Log  in to  Adobe Admin Console](/brand-portal-manage-groups.md#LogintoAdobeAdminConsole).
1. From the toolbar at the top, click **Products**. 
1. In the **Products** page, **Product Profiles** is selected by default. Open the product profile to which you want to add a user, for example, **Sales group**.

   ![](assets/admin_console_productprofileadded.png)

1. To add individual users to the product profile, do the following:

    * Click **Add User**.

   ![](assets/admin_console_productprofilesalesgroup.png)

    * In the **Add User to Sales group** page, type the email ID of the user you want to add or select the user from the list of suggestions that appear as you type.

   ![](assets/admin_console_addusertosalesgroup.png)

    * Click **Save**.

1. To add bulk users to the product profile, do the following:

    * Choose ellipsis (**...**) &gt; **Add users by CSV**.

   ![](assets/admin_console_addbulkusers.png)

    * In the **Add Users by CSV** page, download a CSV template or drag-and-drop a CSV file.

   ![](assets/admin_console_addbulkuserscsv.png)

    * Click **Upload**.

   If you added users to the default product profile, that is, Assets Brand Portal, a welcome email is sent to the email ID of the users you added. The invited users can access Brand Portal by clicking the link in the welcome email and signing in using an Adobe ID. For more information, see [First-time login experience](/brand-portal-onboarding.md).

   Users added to a custom or a new product profile do not receive email notifications.

