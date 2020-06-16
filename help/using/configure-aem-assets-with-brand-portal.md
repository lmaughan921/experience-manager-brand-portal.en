---
title: Configure AEM Assets with Brand Portal
seo-title: Configure AEM Assets with Brand Portal
description: Get an insight into configuring AEM Assets with Brand Portal.
seo-description: Get an insight into configuring AEM Assets with Brand Portal.
uuid: 
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 
---

# Configure AEM Assets with Brand Portal {#configure-integration}

Adobe Experience Manager (AEM) Assets is configured with Brand Portal via Adobe Developer Console, which procures an IMS token for authorization of your Brand Portal tenant. Brand Portal is now supported on AEM Assets cloud service, AEM Assets 6.3 and above. 

Configuring AEM Assets could service with Brand Portal allows you to publish and distribute assets with the Brand Portal users. Whereas, Configuring Brand Portal on AEM 6.3 (and above) enables asset publishing, asset distribution and asset contribution features for the Brand Portal users.

>[!NOTE]
 >
 >***For AEM Assets 6.3 and above***
 >
 >Earlier, Brand Portal was configured in Classic UI via Legacy OAuth Gateway, which uses the JWT token exchange to obtain an IMS Access token for authorization. 
 >
 >Configuration via Legacy OAuth is no longer supported from April 6, 2020, and is changed to configuring via Adobe Developer Console.
 >

>[!TIP]
 >
 >***For existing customers only*** 
 >
 >Legacy OAuth Gateway configuration will continue working for existing customers. 
 >
 >In case you encounter problems with legacy OAuth Gateway configuration, delete the existing configuration and create new configuration via Adobe Developer Console.
 >

The steps to configure AEM Assets with Brand Portal are different depending on your AEM version, and whether you are configuring for the first-time, or upgrading the existing configurations:

| **AEM Version** |**New Configuration** |**Upgrade Configuration** |
|---|---|---|
| **AEM Assets as a Cloud Service** |[Create configuration](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) |- |
| **AEM 6.5 (6.5.4.0 and above)** |[Create configuration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) |[Upgrade configuration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) | 
| **AEM 6.4 (6.4.8.0 and above)** |[Create configuration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) |[Upgrade configuration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) | 
| **AEM 6.3 (6.3.3.8 and above)** |[Create configuration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) |[Upgrade configuration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) | 
| **AEM 6.2** |Contact Support |Contact Support | 


