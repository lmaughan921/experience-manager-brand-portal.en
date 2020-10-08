---
title: Manage users, groups, and user roles
seo-title: Manage users, groups, and user roles
description: Administrators can use Adobe Admin Console to create AEM Assets Brand Portal users and product profiles, and manage their roles using the Brand Portal user interface. This privilege is not available to Viewers and Editors.
seo-description: Administrators can use Adobe Admin Console to create AEM Assets Brand Portal users and product profiles, and manage their roles using the Brand Portal user interface. This privilege is not available to Viewers and Editors.
uuid: 0dc1867c-6d1b-4d0d-a25e-0df207c269b8
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: ba468e80-d077-4af6-b782-238fc557e22b
---

# Manage Users, Groups, and User Roles {#manage-users-groups-and-user-roles}

Administrators can use Adobe Admin Console to create AEM Assets Brand Portal users and product profiles, and manage their roles using the Brand Portal user interface. This privilege is not available to Viewers and Editors.

In [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview), you can view all the products associated with your organization. A product could be any Experience Cloud solution, such as Adobe Analytics, Adobe Target, or AEM Brand Portal. You must choose the AEM Brand Portal product, and create Product Profiles.

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

These product profiles are synced with the Brand Portal user interface every 8 hours and visible as groups in Brand Portal. Once you add users and create product profiles, and add users to those product profiles, you can assign roles to users and groups in Brand Portal.

>[!NOTE]
>
>To create groups in Brand Portal, from Adobe [!UICONTROL Admin Console], use **[!UICONTROL Products > Product Profiles]**, instead of **[!UICONTROL User page > User Groups]**. Product profiles in Adobe [!UICONTROL Admin Console] are used to create groups in Brand Portal.

## Add a user {#add-a-user}

If you are a product administrator, use Adobe [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) to create users and assign them to product profiles (*formerly known as product configurations*), which show as groups in Brand Portal. You can use groups to perform bulk operations such as role management and asset sharing.

>[!NOTE]
>
>New users who do not have access to Brand Portal can request access from the login screen of Brand Portal. For more information, refer to [Request access to Brand Portal](../using/brand-portal.md#request-access-to-brand-portal). After you receive access request notifications in your notification area, click the relevant notification and then click **[!UICONTROL Grant Access]**. Alternatively, follow the link in the access request email received. Next, to add a user through [Adobe [!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview), follow Steps 4-7 in the procedure below.

>[!NOTE]
>
>You can login to [Adobe [!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directly or from Brand Portal. If you login directly, follow Steps 4-7 in the procedure below to add a user.

1. From the AEM toolbar at the top, click the Adobe logo to access administrative tools.

   ![AEM logo](assets/aemlogo.png)

1. From the administrative tools panel, click **[!UICONTROL Users]**.

   ![Admin tools panel](assets/admin-tools-panel-5.png)

1. In the [!UICONTROL User Roles] page, click the **[!UICONTROL Management]** tab, then click **[!UICONTROL Launch Admin Console]**.

   ![User Roles to launch Admin Console](assets/launch_admin_console.png)

1. In Admin Console, do one of the following to create a new user:

    * From the toolbar at the top, click **[!UICONTROL Overview]**. In the [!UICONTROL Overview] page, click **[!UICONTROL Assign Users]** from the Brand Portal product card.

   ![Admin Console Overview](assets/admin_console_overviewadduser.png)

    * From the toolbar at the top, click **[!UICONTROL Users]**. In the [!UICONTROL Users] page, [!UICONTROL Users] in the left rail is selected by default. Click **[!UICONTROL Add User]**.

   ![Admin Console Add users](assets/admin_console_adduseruserpage.png)

1. In the add user dialog box, type the email ID of the user you want to add or select the user from the list of suggestions that appear as you type.

   ![Add user to Brand Portal](assets/add_user_to_aem_bp.png)

1. Assign the user to at least one product profile (formerly known as product configurations) so that the user can access Brand Portal. Select the appropriate product profile from the **[!UICONTROL Please select a profile for this product]** field.
1. Click **[!UICONTROL Save]**. A welcome email is sent to the user you added. The invited user can access Brand Portal by clicking the link in the welcome email and signing in using an [!UICONTROL Adobe ID]. For more information, see [First-time login experience](../using/brand-portal-onboarding.md).

   >[!NOTE]
   >
   >If a user is unable to log on to Brand Portal, the Administrator of the organization should visit Adobe [!UICONTROL Admin Console] and check whether the user is present and has been added to at least one product profile.

   For information about granting administrative privileges to the user, see [Provide administrator privileges to users](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## Add a product profile {#add-a-product-profile}

Product profiles (formerly known as product configurations) in [!UICONTROL Admin Console] are used to create groups in Brand Portal so that you can perform bulk operations such as role management and asset sharing in Brand Portal. **Brand Portal** is the default product profile available; you can create more product profiles and add users to the new product profiles.

>[!NOTE]
>
>You can login to [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directly or from Brand Portal. If you login to [!UICONTROL Admin Console] directly, follow Steps 4-7 in the procedure below to add a product profile.

1. From the AEM toolbar at the top, click the Adobe logo to access administrative tools.

   ![AEM Logo](assets/aemlogo.png)

1. From the administrative tools panel, click **[!UICONTROL Users]**.

   ![Admin tools panel](assets/admin-tools-panel-6.png)

1. In the [!UICONTROL User Roles] page, click the **[!UICONTROL Management]** tab, then click **[!UICONTROL Launch Admin Console]**.

   ![Launch Admin Console](assets/launch_admin_console.png)

1. From the toolbar at the top, click **[!UICONTROL Products]**.
1. In the [!UICONTROL Products] page, [!UICONTROL Product Profiles] is selected by default. Click **[!UICONTROL New Profile]**.

   ![Add new Product Profile](assets/admin_console_addproductprofile.png)

1. In the [!UICONTROL Create a New Profile] page, provide the profile name, display name, profile description, and choose if you want to notify users by email when they are added to or removed from the profile.

   ![Create Product Profile](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. Click **[!UICONTROL Done]**. The product configuration group, for example **[!UICONTROL Sales group]**, is added to Brand Portal.

   ![Product profiles](assets/admin_console_productprofileadded.png)

## Add users to a product profile {#add-users-to-a-product-profile}

To add users to a Brand Portal group, add them to the corresponding product profile (formerly known as product configurations) in [!UICONTROL Admin Console]. You can add users individually or in bulk.

>[!NOTE]
>
>You can login to [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directly or from Brand Portal. If you login to Admin Console directly, follow Steps 4-7 in the procedure below to add users to a product profile.

1. From the AEM toolbar at the top, click the Adobe logo to access administrative tools.

   ![AEM Logo](assets/aemlogo.png)

1. From the administrative tools panel, click **[!UICONTROL Users]**.

   ![Admin tools panel](assets/admin-tools-panel-7.png)

1. In the [!UICONTROL User Roles] page, click the **[!UICONTROL Management]** tab, then click **[!UICONTROL Launch Admin Console]**.

   ![Launch [!DNL Admin Console]](assets/launch_admin_console.png)

1. From the toolbar at the top, click **[!UICONTROL Products]**.
1. In the [!UICONTROL Products] page, [!UICONTROL Product Profiles] is selected by default. Open the product profile to which you want to add a user, for example, [!UICONTROL Sales group].

   ![Product profiles](assets/admin_console_productprofileadded.png)

1. To add individual users to the product profile, do the following:

    * Click **[!UICONTROL Add User]**.

   ![Group to map Product Profile in Brand Portal](assets/admin_console_productprofilesalesgroup.png)

    * In the [!UICONTROL Add User to Sales group] page, type the email ID of the user you want to add or select the user from the list of suggestions that appear as you type.

   ![Add user to a group](assets/admin_console_addusertosalesgroup.png)

    * Click **[!UICONTROL Save]**.

1. To add bulk users to the product profile, do the following:

    * Choose **[!UICONTROL ellipsis (...) > Add users by CSV]**.

   ![Add users in bulk](assets/admin_console_addbulkusers.png)

    * In the **[!UICONTROL Add Users by CSV]** page, download a CSV template or drag-and-drop a CSV file.

   ![Add users by csv](assets/admin_console_addbulkuserscsv.png)

    * Click **[!UICONTROL Upload]**.

   If you added users to the default product profile, that is, Brand Portal, a welcome email is sent to the email ID of the users you added. The invited users can access Brand Portal by clicking the link in the welcome email and signing in using an [!UICONTROL Adobe ID]. For more information, see [First-time login experience](../using/brand-portal-onboarding.md).

   Users added to a custom or a new product profile do not receive email notifications.

## Provide administrator privileges to users {#provide-administrator-privileges-to-users}

You can provide the system administrator or the product administrator privilege to a Brand Portal user. Do not provide other administrative rights available in [!UICONTROL Admin Console], such as product profile administrator, user group administrator, and support administrator. To know more about these roles, see [Administrative roles](https://helpx.adobe.com/enterprise/using/admin-roles.html).

>[!NOTE]
>
>You can login to [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) directly or from Brand Portal. If you login to [!UICONTROL Admin Console] directly, follow Steps 4-8 in the procedure below to add a user to a product profile.

1. From the AEM toolbar at the top, click the Adobe logo to access administrative tools.

   ![AEMLogo](assets/aemlogo.png)

1. From the administrative tools panel, click **[!UICONTROL Users]**.

   ![Admin tools panel](assets/admin-tools-panel-8.png)

1. In the [!UICONTROL User Roles] page, click the **[!UICONTROL Management]** tab, then click **[!UICONTROL Launch Admin Console]**.

   ![Launch Admin Console](assets/launch_admin_console.png)

1. From the toolbar at the top, click **[!UICONTROL Users]**.
1. In the [!UICONTROL Users] page, [!UICONTROL Users] in the left rail is selected by default. Click the user name of the user to whom you want to provide administrator privileges.

   ![Add Users in Admin Console](assets/admin_console_adduseruserpage.png)

1. In the user profile page, locate the **[!UICONTROL Administrative Rights]** section at the bottom, and choose **[!UICONTROL ellipsis (...) > Edit admin rights]**.
   ![Admin rights in Admin Console](assets/admin_console_editadminrights.png)

1. In the [!UICONTROL Edit Admin] page, select System Administrator or Product Administrator.

   ![Edit admin rights in Admin Console](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   >
   >Brand Portal supports only System Administrator and Product Administrator roles.
   >
   >Adobe recommends that you avoid using the System Administrator role because it grants organization-wide administrator privileges for all the products of an organization. For example, a system administrator of an organization that includes three marketing cloud products has the entire set of privileges for all three products. Only a System Administrator can configure AEM Assets so that assets can be published from AEM Assets to Brand Portal. For more information, see [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
   >
   >In contrast, the Product Administrator role grants administrator privileges for a specific product only. If you want to enforce a more granular access control within Brand Portal, use the Product Administrator role and select the product as Brand Portal.

   >[!NOTE]
   >
   >Brand Portal does not support product profile administrator (formerly known as configuration administrator) privileges. Avoid assigning product profile administrator rights to a user.

1. Review the admin type selection and click **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >To revoke administrator privileges for a user, make the appropriate changes in the **[!UICONTROL Edit Admin]** page, and then click **[!UICONTROL Save]**.

## Manage user roles {#manage-user-roles}

An Administrator can modify roles for users in Brand Portal.

In addition to the Administrator role, Brand Portal supports the following roles:

* [!UICONTROL Viewer]: Users with this role can view the files and folders that an Administrator shares with them. Viewers can also search and download assets. However, Viewers cannot share content (files, folders, [!UICONTROL collections]) with other users.
* [!UICONTROL Editor]: Users with this role has all the privileges of a Viewer. In addition, Editors can share content (folders, [!UICONTROL collections], links) with other users.

1. From the AEM toolbar at the top, click the Adobe logo to access administrative tools.

   ![AEMLogo](assets/aemlogo.png)

1. From the administrative tools panel, click **[!UICONTROL Users]**.

   ![Admin tools panel](assets/admin-tools-panel-9.png)

1. In the [!UICONTROL User Roles] page, the [!UICONTROL Users] tab is selected by default. For the user whose role you want to change, select **[!UICONTROL Editor]** or **[!UICONTROL Viewer]** from the **[!UICONTROL Role]** drop-down.

   ![Modify users roles](assets/modify_user_role.png)

   To modify the role of multiple users simultaneously, select the users and choose the appropriate role from the **[!UICONTROL Role]** drop-down.

   >[!NOTE]
   >
   >The [!UICONTROL Role] list for Administrator users is disabled. You cannot select these users to modify their roles.

   >[!NOTE]
   >
   >The user role is also disabled if the user is a member of the Editor group. To revoke editing privileges from the user, either remove the user from the Editor group or change the role of the entire group to Viewer.

1. Click **[!UICONTROL Save]**. The role is modified for the corresponding user. If you selected multiple users, the roles for all the users are modified simultaneously.

   >[!NOTE]
   >
   >Changes in user permissions are reflected in the **[!UICONTROL User Roles]** page only after the users re-login to Brand Portal.

## Manage group roles and privileges {#manage-group-roles-and-privileges}

An Administrator can associate specific privileges with a [group](../using/brand-portal-adding-users.md#main-pars-title-278567577) of users on Brand Portal. The **[!UICONTROL Groups]** tab on the **[!UICONTROL User Roles]** page allows administrators to:

* Assign roles to user groups
* Restrict user groups to download original renditions of image files (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) from Brand Portal.

>[!NOTE]
>
>For the assets shared as the link, the permission to access original renditions of image files will apply based on the permissions of the user who is sharing the assets.

To modify the role and right to access original renditions for specific group members, follow these steps:

1. On the **[!UICONTROL User Roles]** page, navigate to the **[!UICONTROL Groups]** tab.
1. Select the groups for which you want to change roles.
1. Select the appropriate role from the **[!UICONTROL Role]** drop-down list.

   To allow the members of a group to have access to original renditions of image files (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) which they download from the portal or shared link, keep the **[!UICONTROL Access to  Original]** option selected for that group. By default, **[!UICONTROL Access to Original]** option is selected for all the users. To prevent a user group from accessing original renditions, deselect the option corresponding to that group.

   ![User group roles](assets/access-original-rend.png)

   >[!NOTE]
   >
   >If a user is added to multiple groups and if one of these groups has restrictions, the restrictions will apply to that user.
   >
   >Also, restrictions to access original renditions of image files do not apply to administrators even though they are members of restricted groups.

1. Click **[!UICONTROL Save]**. The role is modified for the corresponding groups.

   >[!NOTE]
   >
   >The user-to-group association, or the group membership of a user, is synced to  Brand Portal every 8 hours. Changes to user or group roles are effective after the next sync job runs.
