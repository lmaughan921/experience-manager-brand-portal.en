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
   >If you are an existing customer, it is recommended to continue using existing legacy OAuth Gateway configuration. In case, you encounter problems with legacy OAuth Gateway configuration,  delete the existing configuration and create new configuration via Adobe I/O.
   >

The steps to configure AEM Assets with Brand Portal are different depending on your AEM version, and whether you are configuring for the first-time, or upgrading the existing configurations:

| **AEM Version** |**New Configuration** |**Upgrade Configuration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 and above)** |[Create configuration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) |[Upgrade configuration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) | 
| **AEM 6.4 (6.4.8.0 and above)** |[Create configuration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) |[Upgrade configuration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) | 
| **AEM 6.3 (6.3.3.8 and above)** |[Create configuration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) |[Upgrade configuration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) | 
| **AEM 6.2** |Contact Support |Contact Support | 


<!--
   Comment Type: draft

   <li> </li>
   -->

   <!--
   Comment Type: draft

   <li>Step text</li>
   -->
