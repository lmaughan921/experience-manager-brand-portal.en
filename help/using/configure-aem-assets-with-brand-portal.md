---
title: Configure AEM Assets with Brand Portal
seo-title: Configure AEM Assets with Brand Portal
description: Get an insight into configuring AEM Assets with Brand Portal.
seo-description: Get an insight into configuring AEM Assets with Brand Portal.
uuid: 
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 
---

# Configure AEM Assets with Brand Portal {#configure-integration}

Adobe Experience Manager (AEM) Assets is configured with Brand Portal through Adobe I/O, which procures an IMS token for authorization of your Brand Portal tenant. The configuration enables asset publishing, asset distribution and asset contribution features for the Brand Portal users.

>[!NOTE]
   >
   >Earlier, Brand Portal was configured in Classic UI via Legacy OAuth Gateway, which uses the JWT token exchange to obtain an IMS Access token for authorization. 
   >
   >Configuration via Legacy OAuth is no longer supported from April 6, 2020, and is changed to configuring via Adobe I/O.
   >
   >If you are an existing Brand Portal user with configuration on legacy OAuth Gateway, it is recommended to delete the existing configurations and create new configuration on Adobe I/O.
   >
   >However, the existing configuration will continue to work if you do not modify the configurations.

The steps to configure AEM Assets with Brand Portal are different depending on your AEM version, and whether you are configuring for the first-time, or upgrading the existing configurations:

| **AEM Version** |**New Configuration** |**Upgrade Configuration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-65.md) |[Upgrade configuration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4 (6.4.8.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-64.md) |[Upgrade configuration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3 (6.3.3.8 and above)** |[Create configuration](../using/brand-portal-configure-integration-63.md) |[Upgrade configuration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 


<!--
   Comment Type: draft

   <li> </li>
   -->

   <!--
   Comment Type: draft

   <li>Step text</li>
   -->
