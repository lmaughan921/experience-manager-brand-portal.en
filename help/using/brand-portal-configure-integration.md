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

# Configure AEM Assets with Brand Portal {#configure-integration}

Adobe Experience Manager (AEM) Assets is configured with Brand Portal through Adobe I/O which procures an IMS token for authorization of your Brand Portal tenant. 

>[!NOTE]
   >
   >Earlier, Brand Portal was configured in Classic UI via Legacy OAuth Gateway, which uses the JWT token exchange to obtain an IMS Access token for authorization.
   >
   >Configuration via Legacy OAuth is no longer supported from April 6, 2020, and is shifted to Adobe I/O.
   >
   >However, the existing configuration will continue to work if you do not modify the configurations.

This help describes the following two use-cases: 
* If you are a new Brand Portal user and want to configure your AEM Assets author instance with Brand Portal, you can create new configuration on Adobe I/O. 
* If you are an existing Brand Portal user with your AEM Assets author instance configured with Brand Portal on legacy OAuth Gateway, it is recommended to delete the existing configuration and create new configuration on Adobe I/O.

The steps to configure AEM Assets with Brand Portal are different depending on your AEM version, and whether you are configuring for the first-time, or upgrading the existing configurations:

| **AEM Version** |**New Configuration** |**Upgrade Configuration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 and above)** |[Create new configuration](../using/brand-portal-configure-integration-65.md) |[Upgrade existing configurations](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4 (6.4.8.0 and above)** |[Create new configuration](../using/brand-portal-configure-integration-64.md) |[Upgrade existing configurations](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3 (6.3.3.8 and above)** |[Create new configuration](../using/brand-portal-configure-integration-63.md) |[Upgrade existing configurations](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 

The information provided is based on the assumption that anyone reading this Help is familiar with the following technologies:

* Installing, configuring, and administering Adobe Experience Manager and AEM packages

* Using Linux and Microsoft Windows operating systems

## Prerequisites {#prerequisites}

You require the following to configure AEM Assets with Brand Portal:

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

**Contact Support** if you are unable to find the latest AEM package or Service Pack.


<!--
   Comment Type: draft

   <li> </li>
   -->

   <!--
   Comment Type: draft

   <li>Step text</li>
   -->
