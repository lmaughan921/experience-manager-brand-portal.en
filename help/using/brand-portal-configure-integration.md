---
title: Configure AEM Assets integration with Brand Portal
seo-title: Configure AEM Assets integration with Brand Portal
description: Get an insight into configuring integration of AEM Assets with Brand Portal.
seo-description: Get an insight into configuring integration of AEM Assets with Brand Portal.
uuid: 
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 
---

# Configure AEM Assets integration with Brand Portal {#configure-integration}

Adobe Experience Manager (AEM) Assets is integrated with Brand Portal which enables asset publishing, asset distribution and asset contribution features.

This help describes the following two use-cases: 
* If you are a new Brand Portal user and want to integrate your AEM Assets author instance with Brand Portal. 
* If you are an existing Brand Portal user having your AEM Assets author instance integrated with Brand Portal. 

>[!NOTE]
   >
   >Integration via Adobe I/O Console is supported on AEM 6.3 and above.

The information provided is based on the assumption that anyone reading this Help is familiar with the following technologies:

* Installing, configuring, and administering Adobe Experience Manager and AEM packages

* Using Linux and Microsoft Windows operating systems

## How integration works? {#how-integration-works}

AEM Assets is integrated with Brand Portal through Adobe I/O Console which procures IMS token for authentication of your Brand Portal tenant. 

>[!NOTE]
   >
   >Earlier, Brand Portal was configured in Classic UI via Legacy OAuth Gateway which uses the JWT token exchange to obtain an IMS Access token for authorization.
   >
   >Integration with Legacy OAuth is no longer supported from April 6, 2020, and is shifted to Adobe I/O Console.
   >
   >But, the existing configuration will continue to work if you do not modify the integration. You will be able to  publish assets from AEM Assets to Brand Portal without modifying the integration.
   >
   >Follow this HELP to upgrade your integration settings to Adobe I/O Console, or create new integration.  


## Prerequisites {#prerequisites}

You require the following to configure AEM Assets integration with Brand Portal:

* An up and running AEM Assets author instance with latest Service Pack.
* Brand Portal tenant URL.
* A user with system administrator privileges on the IMS organization of the Brand Portal tenant. 


[Download and install AEM 6.5 or AEM 6.4](#aemquickstart)

[Download and install latest AEM Service Pack](#servicepack)

### Download and install AEM 6.5 or AEM 6.4 {#aemquickstart}

Brand Portal is integrated with AEM Assets. It is recommended to have AEM 6.5 or AEM 6.4 to set up an AEM author instance. If you do not have AEM up and running, download it from the following locations:

* If you are an existing AEM customer, download AEM 6.5, AEM 6.4, or AEM 6.3 from [Adobe Licensing website](http://licensing.adobe.com).

* If you are an Adobe partner, use [Adobe Partner Training Program](https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=82357Q) to request AEM 6.5, AEM 6.4, or AEM 6.3.

After you download AEM, for instructions to set up an AEM author instance, see [deploying and maintaining](https://helpx.adobe.com/experience-manager/6-5/sites/deploying/using/deploy.html#defaultlocalinstall).

### Download and install AEM latest Service Pack {#servicepack}

Download and install latest AEM Service Pack. 

For detailed instructions see, 

* [AEM 6.5 Service Pack Release Notes](https://helpx.adobe.com/experience-manager/6-5/release-notes/sp-release-notes.html) 
* [AEM 6.4 Service Pack Release Notes](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html)
* [AEM 6.3 Cumulative Fix Pack](https://helpx.adobe.com/experience-manager/release-notes--aem-6-3-cumulative-fix-pack.html)

## Configure integration {#configure-integration-bp}

The steps to configure integration are different depending on your AEM version, and whether you are configuring integration for the first-time, or upgrading the existing integration:

| **AEM Version** |**Configure New Integration** |**Upgrade Integration** |
|---|---|---|
| **AEM 6.5 or AEM 6.4** |[Create new integration](../using/brand-portal-configure-integration-65.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65-64) | 
| **AEM 6.3** |[Create new integration](#configure-new-integration-65-64) |[Upgrade existing integration](#upgrade-existing-integration-65-64) | 
| **AEM 6.2** |Contact Support |Contact Support | 
 

>[!NOTE]
   >
   >The existing configurations will continue work if you do not modify the integration.

<!--
   Comment Type: draft

   <li> </li>
   -->

   <!--
   Comment Type: draft

   <li>Step text</li>
   -->
