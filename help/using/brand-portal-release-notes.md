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

Brand Portal 6.4.5 is a feature release that focuses on providing Brand Portal users (external agencies/teams) with the ability to upload content to Brand Portal and publish to AEM Assets, without needing access to the author environment. This feature is called **Asset Sourcing in Brand Portal**, and will improve customer experiences by providing a two-way mechanism for users to both contribute and share assets with other globally distributed Brand Portal users.

**Asset Sourcing in Brand Portal**

Asset Sourcing allows AEM administrators to create new folders with an additional **Asset Contribution** property, ensuring the new folder created open to asset submission by Brand Portal users. This automatically triggers a workflow which creates two additional sub folders, called NEW and SHARED, within the newly created **Contribution** folder.

The AEM Administrator then defines the requirement by uploading a brief about the types of assets that should be added to the contribution folder, as well as a set of baseline assets, to the **SHARED** folder to ensure BP users have the reference information they need. The administrator can then grant active Brand Portal users access to the contribution folder before publishing the newly created **Contribution** folder to Brand Portal.

Once the user is finished adding content in the **NEW** folder, they can publish the contribution folder back to the AEM author environment.

In order to use the Asset Sourcing feature, following capabilities are available in AEM and Brand Portal:

**Capabilities in AEM**

* **Enable Asset Sourcing configuration flag**: Administrators can enable the Asset Sourcing flag from the AEM Configuration Manager.

* **Create and share contribution folder**: Administrators/editors can create new folders with an additional **Asset Contribution** property and share it with the active Brand Portal users for contribution.

* **Pulse/email notifications**: AEM Administrator receive pulse/email notifications both at the beginning and at the completion of the publish action.

* **View job status**: Administrators/editors can view the status (Queued/In-progress/Success) of the import job.

**Capabilities in Brand Portal**

* **Pulse/email notifications**: Brand Portal users receive notifications when a contribution folder is shared with them, on publishing the contribution folder to AEM, and at the completion of the publish action.

* **Download asset requirements**: Brand Portal users can download the brief document, as well as download the baseline content, from the **SHARED** folder to ensure they understand the asset requirements.

* **Upload new assets to contribution folder**: Brand Portal users can upload content (assets/folders containing multiple assets) in the **NEW** folder.

* **Publish contribution folder to AEM Assets**: Brand Portal users manually publishes the contribution folder to AEM Assets.

* **View job status**: Brand Portal administrators can view the status (Queued/In-progress/Success) of the publish action.

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
