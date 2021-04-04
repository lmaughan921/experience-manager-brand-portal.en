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
role: Administrator
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
---
# Configure AEM Assets with Brand Portal {#configure-integration}

Configuring Adobe Experience Manager Assets with Brand Portal enables asset publishing, asset distribution, and asset contribution features for the Brand Portal users. It allows the AEM Assets users to publish and distribute assets with the Brand Portal users. The Brand Portal users can access the shared assets and contribute by uploading new assets to the asset contribution folders and publishing them back to AEM Assets. 

Configuring AEM Assets with Brand Portal is supported on:
* AEM Assets as a Cloud Service
* AEM Assets (on premise and managed service) 6.3 and above

AEM Assets as a Cloud Service is automatically configured with Brand Portal by activating Brand Portal from the Cloud Manager. The activation workflow creates the required configurations at the backend and activates Brand Portal on the same IMS org as of the AEM Assets as a Cloud Service instance.  

Whereas, AEM Assets (on premise and managed service) is manually configured with Brand Portal using Adobe Developer Console, which procures an Adobe Identity Management Services (IMS) token for authorization of the Brand Portal tenant. 

>[!NOTE]
>
>***For AEM Assets 6.3 and above***
>
>Earlier, Brand Portal was configured in classic interface via Legacy OAuth Gateway, which uses the JSON Web token (JWT) exchange to obtain an IMS token for authorization. 
>
>Configuration via Legacy OAuth is no longer supported from April 6, 2020, and is changed to configuring via Adobe Developer Console.


>[!TIP]
>
>***For existing customers only (on premise and managed service)*** 
>
>Legacy OAuth Gateway configuration will continue working for existing customers. 
>
>In case you encounter problems with legacy OAuth Gateway configuration, delete the existing configuration and create new configuration via Adobe Developer Console.

The steps to configure AEM Assets with Brand Portal are different depending on your AEM version, and whether you are configuring for the first time, or upgrading the existing configurations:

| **AEM Version** |**New Configuration** |**Upgrade Configuration** |
|---|---|---|
| **AEM Assets as a Cloud Service** |[Activate Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) |- |
| **AEM 6.5 (6.5.4.0 and above)** |[Create configuration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) |[Upgrade configuration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) | 
| **AEM 6.4 (6.4.8.0 and above)** |[Create configuration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) |[Upgrade configuration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) | 
| **AEM 6.3 (6.3.3.8 and above)** |[Create configuration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) |[Upgrade configuration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) | 
| **AEM 6.2** |Contact Support |Contact Support |
