---
title: Release Notes
seo-title: Release Notes
description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.2 release.
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.2 release.
page-status-flag: de-activated
uuid: 80dc8c96-30d5-4d77-b959-dd92c5bc13ee
acrolinxdate: 2018-05-09T09 16 27.606-0400
acrolinxlastcheckedby: mgulati
acrolinxpagestatus: green
acrolinxreporturl: http //acrolinx.corp.adobe.com 8031/output/en/brand_portal_release_notes_641_krs_workflow_3f5278c7e8d024ea_75_report.xml
acrolinxsentences: 53
acrolinxwords: 594
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 921e28a9-cce5-44bc-a35c-3b3f3081fca6
isreadyforlocalization: false
unpublishexternaldate: 2018-11-01T20 09 29.826-0400
index: y
internal: n
snippet: y
---

# Release Notes{#release-notes}

Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.2 release.

## Release Information {#release-information}

| Product |Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version |6.4.2 |

## Overview {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal helps you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices. It helps improve the efficiency of asset sharing, accelerates the time-to-market for assets, and reduces the risk of non-compliance and unauthorized access. Brand Portal allows users to browse, search, preview, download, and export assets in corporate-approved formats—anytime, anywhere.

## What's New in 6.4.2 {#what-s-new-in}

### Enhancements {#enhancements}

This release includes the following enhancements:

* Allowed guest access to Brand Portal.
* Provided option to accelerate the download of asset files from Brand Portal and shared links using Aspera file download accelerator.
* Introduced User Logins report to track the login activity of Brand Portal users and measure the usage of the portal.
* Provided option to restrict specific user groups from accessing original renditions of image files (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop), while allowing them to access low-resolution renditions.
* Displayed folder hierarchy information on folder cards in card view for non-admin users (Guest user, Viewer, Editor), to help differentiate the shared child folders with similar names belonging to different parent folders.  
* Introduced Path column in list view to indicate the hierarchy in which a particular asset resides. 
* Added support for non-case sensitive search for property predicate and multi-value property predicate in search Filter.
* Added six new configurations to give greater control to organizations and enable them to cater to individual business needs.
* The UI for configuring oAuth integrations is now hosted in [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/).

Get insights into enhancements at the [What's New](../using/whats-new.md) page.

### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issues:

* The Collection Title field in Create Collection feature is vulnerable to stored XSS.
* Licensed assets are downloaded even on selecting disagree.
* A corrupted zip file is downloaded if a single asset file is downloaded on Microsoft Edge browser.
* Branding configurations (Header, Footer, and Logo) are not updated in the email when a download is performed through email.
* Future dates are not enabled to select in calendar view while selecting end date at the time of creating Expiration report.
* Licensed assets are not being downloaded from Brand Portal.
* Status like approved, rejected are not visible on assets metadata page.
* Multi-value property predicate search keyword has a missing character at the end.
* Request URI too long 414 error is observed on downloading folder having large number of licensed assets.

### Known Issues {#known-issues}

Contact Adobe Support for more information about the following known issues:

* Download of Lightbox collection by a guest user is not tracked in download report.
* Login screen appears for internal and external users when shared link expires, though generated shared links are public by default.

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

