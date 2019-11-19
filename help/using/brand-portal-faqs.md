---
title: Frequently Asked Questions
seo-title: 
description: Get an insight into the frequently asked questions in the Adobe Experience Manager Assets Brand Portal.
seo-description: 
uuid: 
content-type: reference
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 
---

# Frequently Asked Questions {#frequently-asked-questions}

The Brand Portal FAQs focuses on the end-users queries and issues they might encounter while working with the latest AEM Assets Brand Portal 6.4.5 release or earlier versions.



**Ques. What is the major change in Brand Portal 6.4.5 release?**

**Ans.** AEM Assets Brand Portal 6.4.5 is a feature release which allows the Brand Portal users to upload content from wihtin the Brand Portal instance and publish the Contribution folder back to AEM Assets without needing administrator rights.
For more information, see [Asset Sourcing in Brand Portal](brand-portal-asset-sourcing.md).



**Ques. Will I lose access to any existing assets, features, or configurations I have created?**

**Ans.** All of your existing features and configurations remain intact. Your end-users are not impacted, and your content remains intact.



**Ques. When am I moving to the new version of Brand Portal?**

**Ans.** Brand Portal 6.4.5 was released to production in October 2019. And the next Brand Portal version is expected to be released in Q3 2020. 
For updates and version change, it is recommended to track the [Release Notes](brand-portal-release-notes.md) and [What's New in Brand Portal](whats-new.md).



**Ques. Will my users be impacted?**

**Ans.** The Brand Portal 6.4.5 release is exclusively within Brand Portal, so there is no impact to your end-users.



**Ques. Is there any action required on my part as a Brand Portal user?**

**Ans.** Brand Portal 6.4.5 release comes with a new feature named Asset Sourcing. AEM administrator must configure Asset Sourcing feature in AEM Assets to enable the feature for the Brand Portal users. For more information, refer to [Enable Asset Sourcing](brand-portal-configure-asset-sourcing.md).



**Ques. Who can create a Contribution folder?**

**Ans.** Any AEM users can create a new folder in AEM Assets and assign the property **Asset Contribution**. The newly created folder is called as a **Contribution** folder. 
This folder is then shared with the active Brand Portal users for contribution.  



**Ques. What does a Contribution folder contains?**

**Ans.** **Contribution** folder contains two sub-folders **NEW** and **SHARED**. Initially, the NEW folder is blank and the SHARED folder contains the reference content (reusable assets) for the Brand Portal users. 
The Brand Portal users access the **Contribution** folder and upload content in the **NEW** folder.  



**Ques. What is asset requirements w.r.t contribution?**

**Ans.** The **Brief** document attached to the **Contribution** folder and the reference content (reusable assets) uploaded in the **SHARED** folder helps the Brand Portal user to understand the need of contribution and expectations as a contributor, and is collectively called as the asset requirements.  



**Ques. Can I upload assets to any permitted folder?**

**Ans.** Not all the permitted folders. A Brand Portal user can upload content only to the **Contribution** folder which is shared by the AEM or Brand Portal administrator.



**Ques. How do I get access to a Contribution folder?**

**Ans.** You can access a **Contribution** folder only if it has been shared with you. You will get an email/pulse notification whenever a Contribution folder is shared with you. You can either access the Contribution folder via the link shared in the email, or login to your Brand Portal instance and navigate to the bell icon for notfication to access the Contribution folder.  

>[!NOTE]
>
>If you are not an existing Brand Portal user, request the AEM administrator to create your user in the AEM admin console and add your profile to the user configuration file in Brand Portal users list. Refer, [Adding Brand Portal user](brand-portal-configure-asset-sourcing.md). 



**Ques. What is the Format of the CSV file for user import?**

**Ans.** The format is same as what is supported by Admin Console for bulk user import. Email, first name, and last name are mandatory.



**Ques. What populates the list of users (Brand Portal contributors) in the Asset Contribution user drop-down?**

**Ans.** The users in the drop-down are populated from the Brand Portal user configuration (.csv) file uploaded in AEM.



**Ques. Where can I see the status of import and publish jobs?**

**Ans.** In AEM, you can see the status of an import in **async** job page. In Brand Portal, you can see the status of a publish job in **[!UICONTROL Tools > Asset Contribution status]**.



**Ques. What is the frequency of an import job which runs periodically in AEM?**

**Ans.** In AEM, polling is run every 5 mins.



**Ques. Is there any threashold on the number of times a folder can be published from Brand Portal to AEM Assets?**

**Ans.** No, all the assets in the **NEW** folder are published to AEM Assets regardless of the fact they were published earlier. Everytime a **Contribution** folder is published from Brand Portal to AEM Assets, it overrides the content of the **NEW** folder. 



**Ques. How to upload new assets in a Contribution folder?**

**Ans.** Refer to the detailed documentation for [Uploading assets to Contribution folder](brand-portal-upload-assets-to-contribution-folder.md).



**Ques. I do not see thumbnails/previews on the assets uploaded to the NEW folder by a Brand Portal user?**

**Ans.** It is as designed, coz there is no workflow being run at the Brand Portal end.



**Ques. What happens if a folder is published from AEM Assets to Brand Portal that is in flux?**

**Ans.** In AEM, logs are maintained for each time a folder is published to Brand Portal. At the time of publishing, all the assets which are not published to Brand Portal are put in a replication queue. Any asset added to the folder after the publishing job is triggered are not published to Brand Portal. When the AEM user publishes the folder again, only the assets which were not published earlier (existing in replication queue) are published to Brand Portal. 
This holds true for any folder published from AEM Assets to Brand Portal, and SHARED folder within a Contribution folder.



**Ques. Who do I contact with questions?**

**Ans.** Contact your Adobe Account Manager or Customer Support.


>[!NOTE]
>
>Release schedule is tentative and subject to change. Contact your Adobe Account Manager or Customer Support to get the updated release schedule.




## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

These sites are only available to customers. If you are a customer and require access, contact your Adobe account manager.

* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Care](https://helpx.adobe.com/contact.html)
