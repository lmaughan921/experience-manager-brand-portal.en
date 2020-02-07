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

If you are an Adobe Experience Manager (AEM) Assets Brand Portal customer, you can integrate AEM Assets with Brand Portal to enable asset publishing, asset distribution and asset contribution.

This help describes the following two use-case: 
* If you do not have Brand Portal integrated with your AEM Asssets author instance. 
* If you are an existing Brand Portal user having your AEM Assets author instance integrted with Brand Portal. 

>[!NOTE]
   >
   >Integration via Adobe I/O Console Gateway is supported in AEM 6.2 and above .

The information provided is based on the assumption that anyone reading this Help is familiar with the following technologies:

* Installing, configuring, and administering Adobe Experience Manager and AEM packages,

* Using Linux and Microsoft Windows operating systems,

## How integration works? {#how-integration-works}

AEM Assets is integrated with Brand Portal through Adobe I/O Console Gateway which procures IMS token for authentication of your Brand Portal tenant. 

>[!NOTE]
   >
   >Earlier, Brand Portal was configured in Classic UI via Marketing Cloud OAuth Gateway which uses the JWT token exchange to obtain an IMS Access token for authorization.
   >
   >This approach is no longer supported from April, 2020. And shifted to Adobe I/O Console Gateway for integration. 


The steps to configure integration are different depending on your AEM version and whether you are an configuring integration for the first-time, or modifying the existing integration:
* **Configure new integration**
  
  If you are not an existing Brand Portal user and using AEM 6.5 or above, and want to configure integration to enable asset publishing, asset distribution, and asset contribution features. 

* **Configure integration on AEM 6.5 and AEM 6.4**

  If you are an existing Brand Portal user having integration with AEM 6.5 or AEM 6.4. 
  
* **Configure integration on AEM 6.3 and AEM 6.2**
  
  If you are an existing Brand Portal user having integration with AEM 6.5 or AEM 6.4. 

## Prerequisites {#prerequisites}

You require the following to configure integration:

* An up and running AEM Assets author instance with latest Service Pack.
* Brand Portal tenant URL.
* A user with system administrator privileges on the IMS organization of the Brand Portal tenant. 


[Download and install AEM 6.5 or AEM 6.4](#aemquickstart)

[Download and install latest AEM Service Pack](#servicepack)

### Download and install AEM 6.5 or AEM 6.4 {#aemquickstart}

Brand Portal is integrated with AEM Assets. It is recommended to have AEM 6.5 or AEM 6.4 to set up an AEM author instance. If you do not have AEM up and running, download it from the following locations:

* If you are an existing AEM customer, download AEM 6.5 or AEM 6.4 from [Adobe Licensing website](http://licensing.adobe.com).

* If you are an Adobe partner, use [Adobe Partner Training Program](https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=82357Q) to request AEM 6.5 or AEM 6.4.

After you download AEM, for instructions to set up an AEM author instance, see [deploying and maintaining](https://helpx.adobe.com/experience-manager/6-5/sites/deploying/using/deploy.html#defaultlocalinstall).

### Download and install AEM latest Service Pack {#servicepack}

Download and install latest AEM Service Pack. For detailed instructions see, [AEM 6.5 Service Pack Release Notes](https://helpx.adobe.com/experience-manager/6-5/release-notes/sp-release-notes.html) or [AEM 6.4 Service Pack Release Notes](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html).

## Configure New Integration {#steps-to-configure-integration}

Perform the following steps in the listed sequence to configure integration for the first-time users: 
1. Obtain public certificate for authentication on Adobe I/O
1. Create Adobe I/O integration 
1. Create IMS configuration account
1. Configure Brand Portal cloud service

### Create IMS Configuration {#create-ims-configuration}

IMS configuration authenticates your Brand Portal tenant with AEM Assets author instance. 

IMS configuration includes two steps:

* [Obtain public certificate](#public-certificate) 
* [Create IMS Technical Account configuration](#create-ims-account-configuration)

### Obtain public certificate {#public-certificate}

Public certificate allows you to authenticate your profile on Adobe I/O.

1. Login to your AEM Assets author instance
Default URL: http:// localhost:4502/aem/start.html
1. From **Tools** ![Tools](assets/tools.png) panel, navigate to **[!UICONTROL Security]** >> **[!UICONTROL Adobe IMS Configurations]**.

   ![Adobe IMS Technical Account Configuration UI](assets/ims-config1.png)

1. Adobe IMS Configurations page opens.
   
   Click **[!UICONTROL Create]**. 
   
   This will take you to the **[!UICONTROL Adobe IMS Technical Account Configuration]** page.

1. By default, **Certificate** tab opens.

   In **Cloud Solution**, select **[!UICONTROL Adobe Brand Portal]**.  

1. Mark the checkbox **[!UICONTROL Create new certificate]** and specify an **alias** for the certificate. The alias serves as name of the dialog. 

1. Click **[!UICONTROL Create certificate]**. A dialog appears. Click **[!UICONTROL OK]** to generate the public certificate.

   ![Create Certificate](assets/ims-config2.png)

1. Click **[!UICONTROL Download Public Key]** and save the *AEM-Adobe-IMS.crt* certificate file on your machine. The certificate file is used to [create integration on Adobe I/O Console](#createnewintegration).  

   ![Download Certificate](assets/ims-config3.png)

1.  Click **[!UICONTROL Next]**. 

    **Account** tab opens. Here, you create the Adobe IMS Technical Account but for that you will need the integration details. Keep this page open for now.

    Open a new tab and [Create new integration in Adobe Console](#createnewintegration) to get the integration details for IMS Account configurations. 

### Create Adobe I/O integration {#createnewintegration}

Create new integration in Adobe I/O. The integration generates API Key, Client Secret, and Payload (JWT) which is required in setting up the IMS Technical Account configurations.

1. Login to Adobe Console with account having system administrator privileges on the IMS organization of the Brand Portal tenant.

   Default URL: [https://console.adobe.io/](https://console.adobe.io/) 

1. Click **[!UICONTROL Create Integration]**.

1. Select **[!UICONTROL Access an API]**, and click **[!UICONTROL Continue]**.

   ![Create New Integration](assets/create-new-integration1.png)

1. Create a new integration page opens. 
   
   Select your organization from the drop-down list.

   In **[!UICONTROL Experience Cloud]**, Select **[!UICONTROL AEM Brand Portal]** and click **[!UICONTROL Continue]**. 

   If the Brand Portal option is disabled for you, ensure that you have selected correct organization from the drop-down box above the **[!UICONTROL Adobe Services]** option. If you do not know your organization, contact your administrator.

   ![Create Integration](assets/create-new-integration2.png)

1. Specify a name and description for the integration. Click **[!UICONTROL Select a File from your computer]** and upload the `AEM-Adobe-IMS.crt` file downloaded in the [Obtain Public Certificates](#obtainpubliccertificates) section.

1. Select the profile of your organization. 

   Or, select the default profile **[!UICONTROL Assets Brand Portal]** and click **[!UICONTROL Create Integration]**. The integration is created.

1. Click **[!UICONTROL Continue to integration details]** to view the integration information. 

   Copy the **API Key** and **Client Secret** key.

   ![API Key, Client Secret, and payload information of an integration](assets/create-new-integration3.png)

1. Navigate to **[!UICONTROL JWT]** tab, and copy the **[!UICONTROL JWT payload]**.

   This API Key, Client Secret key, and JWT payload information will be used to create IMS configuration on your local machine.

### Create IMS Technical Account Configuration {#create-ims-account-configuration}

Ensure that you have the performed the following steps:
* Obtain public certificate
* Create new integration

**Steps to create IMS account configuration**

1. Open the IMS Configuration page, **[!UICONTROL Accounts]** tab. You kept the page open at the end of section, [Obtain public certificate](#obtainpubliccertificates).

1. Specify a **[!UICONTROL Title]** for the IMS account.

   In **[!UICONTROL Authorization Server]**, enter the URL: [https://ims-na1.adobelogin.com/](https://ims-na1.adobelogin.com/)  

   Paste the API Key, Client Secret, and JWT payload that you have copied in the end of [Create Adobe I/O integration](#createnewintegration).

   Click **[!UICONTROL Create]**.

   The Integration is created.

   ![IMS Account configuration](assets/create-new-integration4.png)

   >[!CAUTION]
   >
   >Create only one IMS configuration. Do not create multiple IMS configuration.

1. Select the IMS configuration and click **[!UICONTROL Check Health]**. A dialog box appears. 

   Click **[!UICONTROL Check]**. On successful connection, the *Token retrieved successfully* message appears.

   ![On successful connection, the token retrieved successfully message appears. ](assets/create-new-integration5.png)

   <br/> <br/>

### Configure the cloud service {#configure-the-cloud-service}

Create a cloud service configuration to connect your AEM Assets author instance to Brand Portal. Perform the following steps to create a cloud service configuration:

1. Login to your AEM Assets author instance

   Default URL: http:// localhost:4502/aem/start.html
1. From **Tools** ![Tools](assets/tools.png) panel, navigate to **[!UICONTROL Cloud Services >> AEM Brand Portal]**.

   Brand Portal Configurations page opens.

1. Click **[!UICONTROL Create]**.

1. Specify a **[!UICONTROL Title]** for the configuration. 

   Select the IMS Configuration that you have created in [Create IMS Technical Account Configuration](#create-ims-account-configuration)
   
   In **[!UICONTROL Service URL]**, enter your Brand Portal tenant URL.   
   
   Click **[!UICONTROL Save and Close]**.

1. Click **[!UICONTROL Save and Close]**. The cloud configuration is created. Your AEM Assets author instance is now integrted with the Brand Portal tenant. 

### Verify the Replication Agents {#verify-replication-agents}

TBD
TBD
TBD
TBD
TBD
TBD
TBD
<!--
   Comment Type: draft

   <li> </li>
   -->

   <!--
   Comment Type: draft

   <li>Step text</li>
   -->
