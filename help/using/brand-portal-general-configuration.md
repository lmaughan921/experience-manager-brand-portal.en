---
title: Administer general tenant configurations
seo-title: Administer general tenant configurations
description: null
seo-description: Configure download acceleration, public smart collection creation, public collection creation, and enable admin users to delete assets on tenants.
uuid: 1207bac2-9be2-4c2f-acfc-7df3e0366c14
acrolinxdate: 2018-08-20T05 36 57.569-0400
acrolinxlastcheckedby: mgulati
acrolinxpagestatus: yellow
acrolinxreporturl: http //acrolinx.corp.adobe.com 8031/output/en/brand_portal_general_configuration_krs_workflow_a9d8be2d910fe9fc_198_report.xml
acrolinxsentences: 36
acrolinxwords: 392
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2db40d67-95a3-4666-b738-6e5f021a9408
isreadyforlocalization: false
index: y
internal: n
snippet: y
---

# Administer general tenant configurations{#administer-general-tenant-configurations}

AEM Assets Brand Portal allows organizations to configure the following capabilities for specific tenants:

* Asset deletion by administrators
* Public collection creation by non-admin users
* Public smart collection creation by non-admin users
* Download acceleration
* Parent hierarchy of shared folders visible to non-admin users

These configurations have been provided as **General Settings **configurations on the administrative tools panel.

![](assets/General-configs.png)

**A** Configuration to allow administrators to delete assets from Brand Portal. (Default is enabled)

**B** Configuration to allow the non-admin users to create public collections. (Default is enabled)

**C **Configuration to allow the non-admin users to create public smart collections. (Default is enabled)

**D** Configuration to allow download acceleration of assets downloaded from the portal and from the shared links. (Default is disabled)

**E** Configuration to display folder hierarchy (from the root) of shared folders to non-admin users (Editors, Viewers, Guest Users). (Default is disabled)

## Enable/ disable General configurations {#enable-disable-general-configurations}

To enable/disable each of these configurations:

1. Log in with administrator privileges.
1. Select the AEM logo to access administrative tools, from the toolbar at the top.
1. From the administrative tools panel, select **General **to open the **General Settings **page.
1. Use the respective toggle switch to enable/ disable any of the General configurations.
1. **Save** the changes.
1. Logout to let the changes take effect.

## Allow admin users to delete assets from Brand Portal {#allow-admin-users-to-delete-assets-from-brand-portal}

**Allow users to delete** configuration enables organizations to allow (or restrict) users with administrator privileges to delete assets and folders from Brand Portal.

## Allow public collections creation by non-admins {#allow-public-collections-creation-by-non-admins}

[Allow public collections creation](/brand-portal-share-collection.md#main-pars_text_1915052376) configuration controls whether non-administrators can create public collections on Brand Portal. The configuration is enabled by default. By disabling the configuration organizations can prevent having numerous public collections on their portal so that system space can be saved.

## Allow public smart collections creation by non-admins {#allow-public-smart-collections-creation-by-non-admins}

[Allow public smart collections creation](/brand-portal-searching.md#main-pars_header_500620467) configuration controls whether non-administrators can save their searches as smart collections and make them public for that tenant. The configuration is enabled by default. By disabling the configuration organizations can prevent having a huge number of public smart collections created by non-admin users on organization's Brand Portal.

## Allow download acceleration {#allow-download-acceleration}

[Allow download acceleration](/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.

## Enable Folder Hierarchy {#enable-folder-hierarchy}

[Enable Folder Hierarchy](/brand-portal-sharing-folders.md#main-pars_header_376109647) configuration allows the administrators to control how the non-admin users (Editors, Viewers, and Guest Users) see the shared folders after logging in.
