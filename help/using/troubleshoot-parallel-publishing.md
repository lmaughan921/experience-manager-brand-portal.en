---
title: Troubleshoot issues in parallel publishing to Brand Portal
seo-title: Troubleshoot issues in parallel publishing to Brand Portal
description: Troubleshoot parallel publishing.
seo-description: Troubleshoot parallel publishing.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
role: Administrator
---

# Troubleshoot issues in parallel publishing to Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal is configured with AEM Assets to have approved brand assets seamlessly ingested (or published) from AEM Assets author instance. Once [configured](../using/configure-aem-assets-with-brand-portal.md), AEM Author uses a replication agent to replicate the selected asset(s) to Brand Portal cloud service for approved usage by Brand Portal users. Multiple replication agents are used AEM 6.2 SP1-CFP5, AEM CFP 6.3.0.2, and onwards to allow high-speed parallel publishing.

>[!NOTE]
>
>Adobe recommends upgrading to AEM 6.4.1.0 to ensure that AEM Assets Brand Portal is successfully configured with AEM Assets. A limitation in AEM 6.4 gives an error while configuring AEM Assets with Brand Portal and replication fails.

On configuring cloud service for brand portal under **[!UICONTROL /etc/cloudservice]**, all necessary users and token are auto-generated and saved in the repository. Cloud service configuration is created, service users required for replication and replication agents to replicate content are also created. This creates four replication agents. So when you publish numerous assets from AEM to Brand Portal, these are queued and distributed among these replication agents through Round Robin.

However, publishing can fail intermittently due to- large sling jobs, increased Network and **[!UICONTROL Disk I/O]** on AEM Author instance, or slowed performance of AEM Author instance. It is, therefore, advised to test the connection with the replication agent(s) prior to begin publishing.

![](assets/test-connection.png) 

## Troubleshoot failures in first time publishing: validating your publish configuration {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

To validate your publish configurations:

1. Check the error logs
1. Check whether the replication agent is created
1. Test connection

**Tail logs while creating Cloud Service**

Check tail logs. Check whether the replication agent is created or not. If the replication agent creation fails, edit the cloud service by making minor changes in cloud service. Validate and check again whether the replication agent is created or not. If not, re-edit the service.

If on repeatedly editing the cloud service it is not configured properly, report a daycare ticket.

**Test connection with replication agents**

View log, if errors are found in replication log:

1. Contact Adobe Support.

1. Retry [clean-up](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) and create publish configuration again.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Clean-up existing Brand Portal publish configurations {#clean-up-existing-config}

Most of the times when publishing is not working, the reason can be that the user who is publishing (for example: `mac-<tenantid>-replication` doesn't have the latest private key, and hence publish fails with "401 unauthorized" error and no other error is reported in replication agent logs. You might want to avoid troubleshooting and create a new configuration instead. For the new configuration to work properly, clean up the following from AEM author setup:

1. Go to `localhost:4502/crx/de/` (considering you are running author instance on localhost:4502:  
   i. delete `/etc/replication/agents.author/mp_replication` 
   ii. delete `/etc/cloudservices/mediaportal/<config_name>`

1. Go to localhost:4502/useradmin:  
   i. search for user `mac-<tenantid>replication`
   ii. delete this user

Now the system is all cleaned up. Now you can attempt creating a new  cloudservice  config and still use the already existing JWT application in [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/). There is no need to create a new application, rather just the public key needs to be updated from the newly created cloud config.

## Developer connection JWT application tenant visibility issue {#developer-connection-jwt-application-tenant-visibility-issue}

If on [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/), all the  orgs  (tenants) for which the current users hold system administrator are listed. If you don't find the org name here or you can't create an application for a required tenant here, please check if you have sufficient (system administrator) rights to do this.

There is one known issue on this user interface that for any tenant only top 10 applications are visible. When you create the application, stay on that page and bookmark the URL. You don't need to go to the listing page of the application and find the application that you created. You can hit this bookmarked URL directly and update/delete the application whenever needed.

The JWT application might not be listed appropriately. It is, therefore, advised to note/bookmark the URL while creating JWT application.

## Running Configuration stops working {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

If a replication agent (which was publishing to brand portal just fine) stops processing publish jobs, check replication logs. AEM has auto-retry built-in, so if a particular asset publish fails, it is retried automatically. If there is some intermittent issue like network error, it might succeed during re-try.

If there are continuous publish failures and queue is blocked, then you should check **[!UICONTROL test connection]** and try to solve the errors that are being reported.

Based on the errors, you are advised to log a support ticket, so that Brand Portal engineering team can help you resolve issues.


## Configure replication agents to avoid connection timeout error {#connection-timeout}

Usually the publishing job fails with a timeout error if there are multiple pending requests in the replication queue. To resolve this issue, ensure that the replication agents are configured to avoid timeout. 

Perform the following steps to configure the replication agents:
1. Log in to your AEM Assets author instance.
1. From the **Tools** panel, navigate to **[!UICONTROL Deployment]** > **[!UICONTROL Replication]**.
1. In the Replication page, click **[!UICONTROL Agents on author]**. You can see the four replication agents of your Brand Portal tenant. 
1. Click the replication agent URL to open the agent details.
1. Click **[!UICONTROL Edit]** to modify the replication agent settings.
1. In Agent Settings , click the **[!UICONTROL Extended]** tab. 
1. Select the **[!UICONTROL Close Connection]** check box.
1. Repeat steps 4 through 7 to configure all the four replication agents. 
1. Restart the server.