---
title: Customize wallpaper, header, and email message
seo-title: Customize wallpaper, header, and email message
description: Brand Portal administrators can make limited customizations to the interface displayed to users. You can choose a specific background image (wallpaper) for the Brand Portal login page. You can also add a header image and customize asset sharing emails to match the customer’s brand.
seo-description: Brand Portal administrators can make limited customizations to the interface displayed to users. You can choose a specific background image (wallpaper) for the Brand Portal login page. You can also add a header image and customize asset sharing emails to match the customer’s brand.
uuid: e078d0b9-18b5-467a-ae90-7f0b9fd0d414
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 7b573a4f-2d4e-48d6-b259-436d0cfbdce9
---

# Customize wallpaper, header, and email message{#customize-wallpaper-header-and-email-message}

Brand Portal administrators can make limited customizations to the interface displayed to users. You can choose a specific background image (wallpaper) for the Brand Portal login page. You can also add a header image and customize asset sharing emails to match the customer’s brand.

## Customize the login screen wallpaper {#customize-the-login-screen-wallpaper}

In the absence of a custom branded wallpaper image, a default wallpaper is displayed on the login page.

1. From the AEM toolbar at the top, click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **Branding**.

   ![](assets/admin-tools-panel-10.png)

3. On the left rail of the **Configure Branding** page, **Wallpaper** is selected by default. The default background image that appears on the login page is displayed.

   ![](assets/default_wallpaper.png)

4. To add a new background image, click the **Choose Image** icon from the toolbar at the top.

   ![](assets/choose_wallpaperimage.png)

   Do one of the following:

    * To upload an image from your computer, click **Upload**. Navigate to the required image and upload it.
    * To use an existing Brand Portal image, click **Select from existing**. Choose an image using the asset picker.

   ![](assets/asset-picker.png)

5. Specify a header text and description for the background image. To save the changes, click **Save** from the toolbar at the top.

6. From the toolbar at the top, click the **Preview** icon to generate a preview of the Brand Portal interface with the image.

   ![](assets/chlimage_1.png)
   
   ![](assets/custom-wallpaper-preview.png)

7. To activate or deactivate the default wallpaper, do the following in the **Configure Branding** &gt; **Wallpaper** page:

    * To display the default wallpaper image on the Brand Portal login page, click **Deactivate Wallpaper** from the toolbar at the top. A message confirms that the custom image is deactivated.

   ![](assets/chlimage_1-1.png)

    * To restore the custom image on the Brand Portal login page, click **Activate Wallpaper** from the toolbar. A message confirms that the image is restored.

   ![](assets/chlimage_1-2.png)

    * Click **Save** to save the changes.

## Customize the header {#customize-the-header}

The header appears on various Brand Portal pages after you log in to Brand Portal.

1. From the AEM toolbar at the top, click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **Branding**. 

   ![](assets/admin-tools-panel-11.png)

3. To customize the page header for the Brand Portal interface, on the **Configure Branding** page, select **Header Image** from the left rail. The default header image is displayed.

   ![](assets/default-header.png)

4. To upload a header image, click the **Choose Image** icon and choose **Upload**.

   To use an existing Brand Portal image, choose **Select from existing**.

   ![](assets/choose_wallpaperimage-1.png)

   Choose an image using the asset picker.

   ![](assets/asset-picker-header.png)

5. To include a URL in the header image, specify it in the **Image URL** box. You can specify external or internal URLs. Internal links can also be relative links, for example,
 `/mediaportal.html/content/dam/mac/tenant_id/tags`.
 This link directs users to the tags folder.
 To save the changes, click **Save** from the toolbar at the top.

   ![](assets/configure_brandingheaderimageurl.png)

6. From the toolbar at the top, click the **Preview** icon to generate a preview of the Brand Portal interface with the header image.

   ![](assets/chlimage_1-3.png)
   ![](assets/custom_header_preview.png)

7. To activate or deactivate the header image, do the following in the **Configure Branding** &gt; **Header Image** page:

    * To prevent a header image from appearing on Brand Portal pages, click **Deactivate Header** from the toolbar at the top. A message confirms that the image is deactivated.

   ![](assets/chlimage_1-4.png)

    * To make the header image reappear on Brand Portal pages, click **Activate Header** from the toolbar at the top. A message confirms that the image is activated.

   ![](assets/chlimage_1-5.png)

    * Click **Save** to save the changes.

## Customize the email messaging {#customize-the-email-messaging}

When assets are shared as a link, users receive an email containing the link. Administrators can customize the messaging, that is, logo, description, and footer, of these emails.

1. From the AEM toolbar at the top, click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **Branding**.

   ![](assets/admin-tools-panel-12.png)

3. When assets are shared as links or downloaded through emails, and when collections are shared, email notifications are sent to users. To customize the email message, on the **Configure Branding** page, select **Email Message** from the left rail.

   ![](assets/configure-branding-page-email.png)

4. To add a logo to outgoing emails, click **Upload** from the toolbar at the top.

5. In the **Description** section, specify the email header and footer text. To save the changes, click **Save** from the toolbar at the top.

   >[!NOTE]
   >
   >If you do not use the recommended size for the logo, or if the header and footer text exceed the recommended word count, the content in the email message may appear garbled.
