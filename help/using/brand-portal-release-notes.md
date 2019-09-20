---
title: Release Notes
seo-title: Release Notes
description: Get an insight into the features, enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.5release.
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.5 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
---

# Release Notes {#release-notes}

Get an insight into the new features, enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 6.4.5 release.

## Release Information {#release-information}

| Product |Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 6.4.5|
| Date | September 2019 |

## Overview {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal helps you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices. It helps improve the efficiency of asset sharing, accelerates the time-to-market for assets, and reduces the risk of non-compliance and unauthorized access. Brand Portal allows users to browse, search, preview, download, and export assets in corporate-approved formats—anytime, anywhere.

## What's New in 6.4.5 {#what-s-new-in-645}

### New Features {#new-features-645}

Brand Portal 6.4.5 is a feature release that focuses on providing a collaborative platform for the active Brand Portal users (external agencies/teams) to upload assets in Brand Portal and publish them to AEM Assets without having to access the AEM authoring environment.

**Asset Sourcing in Brand Portal**

The Asset Sourcing feature allows AEM administrators to create new folders with an additional property named–**Asset Contribution**. The new folder created is called as an *Asset Contribution* a.k.a. *Contribution* folder. When a contribution folder is creates, it further contains two sub folders namely–NEW and SHARED. The Brand Portal users who have access to the contribution folder can refer to the baseline assets in the **SHARED** folder and upload assets in the **NEW** folder. After uploading the content, Brand Portal user manually publishes the contribution folder to AEM Assets.

In order to use the Asset Sourcing feature, following capabilities are available in AEM and Brand Portal:

**Capabilities in AEM**

* **Enable Asset Sourcing feature flag**: Administrators can enable the Asset Sourcing flag in AEM Configuration Manager to enable the feature.

* **Create and share contribution folder**: Administrators/editors can create new folders with property—Asset Contribution and share it with the active Brand Portal users for contribution.

* **Pulse/email notifications**: Administrators receive notifications whenever a contribution folder is published from Brand Portal and on completion of the import job.

* **View job status**: Administrators/editors can view the status (Queued/In-progress/Success) of the import job.

**Capabilities in Brand Portal**

* **Pulse/email notifications**: Brand Portal users receive notifications whenever a contribution folder is shared with them, on publishing the contribution folder to AEM, and completion of the publish job.

* **Download project requirement**: Brand Portal users can download the baseline assets from the **SHARED** folder and brief document attached to the contribution folder to understand the project requirement.

* **Upload assets in Brand Portal**: Brand Portal users can access the contribution folder and upload assets (files/folders) in the **NEW** folder.

* **Publish contribution folder to AEM Assets**: Brand Portal users manually publishes the contribution folder to AEM. The ingestion takes place in real-time and reflects the imported assets in AEM Assets.

* **View job status**: Brand Portal administrators can view the status (Queued/In-progress/Success) of the publish job.

For more information, see [What’s New in Brand Portal 6.4.5](whats-new.md).

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
