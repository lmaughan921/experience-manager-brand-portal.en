---
title: Release Notes
seo-title: Release Notes
description: Get an insight into the features, enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.6 release.
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.6 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
---

# Release Notes {#release-notes}

Get an insight into the new features, enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.6 release.

## Release Information {#release-information}

| Product |Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 6.4.6|
| Date | March 2020 |

## Overview {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal helps you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices. It helps improve the efficiency of asset sharing, accelerates the time-to-market for assets, and reduces the risk of non-compliance and unauthorized access. Brand Portal allows users to browse, search, preview, download, and export assets in corporate-approved formats—anytime, anywhere.

## What's New in 6.4.6 {#what-s-new-in-646}

### New Features {#new-feature}

This release includes the following new features:

* Captcha for guest login to Brand Portal. See, [Brand Portal guest access](../using/guest-access.md) for more information.

* Brand Portal is now supported with AEM Assets cloud service. You can configure AEM Assets could service with Brand Portal to share and distribute assets with the Brand Portal users.
  For more information, see [Configure AEM Assets cloud service with Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brandportal/configure-aem-assets-with-brand-portal.html).

### Enhancements {#enhancements-646}

This release of Brand Portal includes the following enhancements:

* In AEM 6.3 and above, the authorization channel between AEM Assets and Brand Portal is changed. AEM Assets is now configured with Brand Portal through Adobe I/O, which procures an IMS token for authorization of your Brand Portal tenant.

  >[!NOTE]
   >
   >Configuration via Legacy OAuth is no longer supported from April 6, 2020, and is changed to configuring via Adobe I/O.
   >


>[!TIP]
>
>***For existing customers only***
>
>It is recommended to continue using existing legacy OAuth Gateway configuration. In case you encounter problems with legacy OAuth Gateway configuration, delete the existing configuration and create a new configuration via Adobe I/O.

For more information, see [Configure AEM Assets with Brand Portal](configure-aem-assets-with-brand-portal.md)

### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issues:

* Metadata schema drop-down values are not visible in asset properties.

* Metadata subschema do not display tabs based on mimetype in asset properties.

* Unpublish metadata schema populates an error message although the schema is removed at backend.

* Preview image do not display for a published asset.

* User is unable to publish or unpublish assets containing single quote in the name.

* Terms and conditions do not display while downloading multiple assets.

* Minor security vulnerabilities addressed.

### Known Issues {#known-issues}

This release includes the following known issues:

* Brand Portal users are not able to publish contribution folder assets to AEM Assets on upgrading to Adobe I/O on AEM 6.5.4.

  This issue will be fixed in the next service pack 6.5.5.

  For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your author instance.

* Exclude System Renditions option is not working properly while downloading an asset.


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

To ascertain which platforms are certified to run with this release of Brand Portal, refer to the **Support for Touch-optimized UI** column in the table in the **Supported Browsers for Authoring User Interface** section of [Technical Requirements](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Links {#links}

* [Adobe Experience Manager Product Page on adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Assets Brand Portal Documentation](https://helpx.adobe.com/experience-manager/brand-portal/user-guide.html)

## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

These sites are only available to customers. If you are a customer and require access, contact your Adobe account manager.

* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Care](https://helpx.adobe.com/contact.html)
