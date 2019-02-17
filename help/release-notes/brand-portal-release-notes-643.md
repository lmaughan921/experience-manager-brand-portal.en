---
title: Release Notes
seo-title: Release Notes
description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.3 release.
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.3 release.
page-status-flag: never-activated
uuid: 82739da5-eb2d-4927-8fac-a1a9a12a70fb
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: bbd005ed-243a-45b9-ad0a-5f4cb2828220
index: y
internal: n
snippet: y
---

# Release Notes{#release-notes}

Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.3 release.

## Release Information {#release-information}

| Product |Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version |6.4.3 |
| Date |November 2018 |

## Overview {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal helps you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices. It helps improve the efficiency of asset sharing, accelerates the time-to-market for assets, and reduces the risk of non-compliance and unauthorized access. Brand Portal allows users to browse, search, preview, download, and export assets in corporate-approved formats—anytime, anywhere.

## What's New in 6.4.3 {#what-s-new-in}

### Enhancements {#enhancements}

This release includes the following enhancements:

* Dynamic media renditions can be downloaded by the users whose AEM Author instance is running on Dynamic Media hybrid mode.
* Dynamic media renditions can be played on asset's card view and previewed on:  
1. asset details page  
  2. link share preview page  
  by the users whose AEM Author instance is running on Dynamic Media hybrid mode.

* Organizations can get their Brand Portal URL customized by having an alternate prefix or a tenant domain alias, by requesting Adobe support.  
  However, AEM Author instance can be configured only with the tenant id URL and not with tenant alias (alternate) URL.
* Publishing/ unpublishing of assets and folders from AEM (6.4.2.0) Author instance to Brand Portal can be scheduled for later.
* Non-admin users (Editors, Viewers, Guest users) can view the shared folders organized in the respective parent directory.
* Path Browser predicate introduced in Search Form to allow searching of assets in a specific directory using the search filter on Brand Portal.
* A configuration has been provided to set up Dynamic Media image server settings.

Get insights into enhancements at the [What's New](../using/whats-new.md) page.

### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issues:

* Fast download using quick action icon in an existing session in shared links prevents download of original renditions.
* Fast download using quick action icon in a new session in shared links causes signout.
* Folders shared through link are not downloaded anonymously.
* Lightbox collection fails to download-- from the action bar.
* Original renditions are downloaded using accelerated download of assets using link share even if the download of original renditions is restricted.
* Fast download using IBM Aspera Connect fails with an error "Your password has expired".
* A blank page opens while downloading the report, having space in its name, from reports listing page.
* Option to remove image presets from Media Portal is not working. 
* Content fails to download if users with non-administrator credentials navigate to a folder using breadcrumbs in column view.
* The "Add to Lightbox" option is not visible on assets on asset search result page on guest access. 
* Download of non-public assets through email link is done by any user through guest access.
* Assets are downloaded through the link shared on email by an unintended user by copying and opening the link in an incognito browser window.
* File names of the files pulled from AEM to Brand Portal lack output encoding.
* Server banner and version are disclosed in application's HTTP response headers, thereby revealing critical information that can let attackers develop further attacks targeted at the specific version of Apache.
* Original assets are downloaded through Shared Link when using IBM Aspera Connect, even if "Allow download of original file" is unchecked at the time of sharing the folder/asset.
* Editors not having access to original renditions see "allow original rendition download" checkbox in link share dialogue.
* Original download restriction alert appears if a user does not select "Asset" checkbox while downloading.
* Settings of a collection, having space at the end of its name, cannot be updated.
* Users logged in as editor/viewer using safari browser cannot create private collection.
* Reports fail to download.
* On a tenant with a large number of users, user report creation take 5 mins with no information on the UI.
* Dispatcher caches the zip file download via email operation is performed. If the same download link is opened the next time, the link is handled by the same dispatcher and no authentication is required to download this time.
* "Header Text" and "Footer" fields are vulnerable to HTML Injection due to lack of output encoding in "Email Message".
* Unauthorized access to Access configuration using Editor, Viewer and Guest user.
* Non-admin users are not able to publish private collection.
* Image presets not working on asset download.
* While sharing assets as a link, entering a name into the user list field display users and groups from other accounts, instead of just those from the currently logged in account.
* A blank page is displayed when the administrator selects Create/Manage Reports.

### Known Issues {#known-issues}

Contact Adobe Support for more information about the following known issues:

* Folder breadcrumb is updated only on the alternate folder if folder hierarchy configuration is enabled.
* Option to Change Thumbnail is visible on video's properties page.
* Lightbox downloads of guest users are not tracked in the Download Report.
* The download via email link contains tenant ID instead of tenant alias, even if the user is logged in through tenant alias.
* Original renditions of dynamic videos do not play on asset detail page.
* [AEM] Path browser predicate is not published on publishing Search Form from AEM Author instance to Brand Portal.
* [AEM] Tag predicates are not published on publishing Metadata Schema Form from AEM Author instance to Brand Portal.

## Languages {#languages}

The Brand Portal user interface is available in following languages:

* English
* German
* French
* Spanish
* Italian
* Brazilian Portuguese
* Japanese
* Simplified Chinese
* Korean

## Certified Platforms {#certified-platforms}

To ascertain which platforms are certified to run with this release of Brand Portal, refer to the **Support for Touch-optimized UI** column in the table in the **Supported Browsers for Authoring User Interface** section of [Technical Requirements](https://docs.adobe.com/content/docs/en/aem/6-3/deploy/technical-requirements.html).

## Links {#links}

* [Adobe Experience Manager Product Page on adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Assets Brand Portal Documentation](https://helpx.adobe.com/experience-manager/brand-portal/user-guide.html)

## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

These sites are only available to customers. If you are a customer and require access, contact your Adobe account manager.

* [](http://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Care](https://helpx.adobe.com/contact.html)

