---
title: Asset Sourcing in Brand Portal
seo-title: Asset Sourcing in Brand Portal
description: Get an insight into the asset sourcing feature released in the Adobe Experience Manager Assets Brand Portal.
seo-description: Get an insight into the asset sourcing feature released in the Adobe Experience Manager Assets Brand Portal.
uuid: 
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 
---

# Asset Sourcing overview {#overview-asset-sourcing-in-bp}

**Adobe Experience Manager (AEM) Assets Brand Portal** focuses on the marketer’s need to effectively collaborate with the globally distributed Brand Portal users by providing a two-way mechanism of asset distribution and asset contribution.

Asset distribution allows you to easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices. Whereas, Asset contribution enables the Brand Portal users with the ability to upload assets to Brand Portal and publish to AEM Assets, without needing access to the author environment. The contribution feature is called as **Assets Sourcing in Brand Portal**. And together, it improves the overall Brand Portal experience of asset distribution and contribution from the Brand Portal users (external agencies/teams), accelerates the time-to-market for assets, and reduces the risk of non-compliance and unauthorized access.

## Why Asset Sourcing? {#asset-sourcing}

**Asset Sourcing** allows AEM administrators to create new folders with an additional **Asset Contribution** property, ensuring the new folder created open to asset submission by Brand Portal users. This automatically triggers a workflow which creates two additional sub folders, called **SHARED** and **NEW**, within the newly created **Contribution** folder. The AEM Administrator then defines the requirement by uploading a brief about the types of assets that should be added to the contribution folder, as well as a set of baseline assets, to the **SHARED** folder to ensure BP users have the reference information they need. The administrator can then grant active Brand Portal users access to the contribution folder before publishing the newly created **Contribution** folder to Brand Portal. Once the user is finished adding content in the **NEW** folder, they can publish the contribution folder back to the AEM author environment. Please note that it may take a few minutes to complete the import and reflect the newly published content within AEM Assets.

Additionally, all existing functionality remains unchanged. Brand Portal users can view, search, and download assets from the contribution folder as well as from the other permitted folders. And administrators can further share the contribution folder, modify properties and add assets to collections.

>[!NOTE]
>
>Asset Sourcing in Brand Portal is supported on AEM 6.5.2.0 and above.
>
>The feature is not supported in the earlier versions - AEM 6.3 and AEM 6.4.

![](assets/asset-sourcing.png)

