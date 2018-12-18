---
title: Brand Portal usage workflows
seo-title: Brand Portal usage workflows
description: Brand Portal usage workflows
seo-description: AEM Brand Portal usage workflows
uuid: 95fc685d-8dee-4bf6-8eb2-4f41bad083a5
contentOwner: mgulati
discoiquuid: 53a7bbb6-be0b-402a-8054-517db44f0d07
---

# Brand Portal usage workflows{#brand-portal-usage-workflows}

This document discusses various workflows in Brand Portal with examples.

## How to restrict access of a user group to a folder? {#how-to-restrict-access-of-a-user-group-to-a-folder}

## Prerequisites

1. Folders
1. Hierarchy as in folder structure
1. User groups

### How

Through ACLs. We can add restrictions to parent folders and not the child folders.

......most open is mostly shared....

## Example

Example and graphic

Our customers are confused in the following scenario:  
let the folder hierarchy be: A &gt; B &gt; C-&gt; D where A is the root.  
now if admin shares B with  groupb , and doesn't share folder C and D with  groupb .  groupb  can still access C & D since they are children of B.  
It is not clear from the current documentation as to how the effective ACLs are calculated for a group on a folder.

we should write a  story line  and explain how can an admin structure their content in the best possible way to take maximum benefit of folder sharing in  Brand  portal.

## How to do

Create a folder structure such that the assets you want to share with non-admin users.

## Why dynamic renditions are empty even after creating image presets? {#why-dynamic-renditions-are-empty-even-after-creating-image-presets}

Why dynamic renditions are not listed on  Asset  Details page.

### Prerequisites

PTIFF on AEM

(Dynamic media settings) Image presets are usable only if Dynamic Media is enabled/on on AEM Author instance. Image presets work on Pyramid Tiff. Pyramid tiff is created when users have dynamic media on/enabled on their AEM Author instance.

### How

How to switch to that mode.

### Example

In the context of image presets.

On Brand Portal, go to an asset and view its Renditions. The image preset created and published from AEM Author is visible under Dynamic within Renditions. While downloading, on download dialog, we have the option to download Dynamic Renditions. Here, we can use the presets already created or specify new presets at run-time.

### How to do

How does it work?

## Sharing assets collections to a group of users

OR why do I see a discrepancy between users in admin console v/s users in AEM Brand Portal? 

How do I share assets or collections to a group of users?

### Prerequisites

### How

What we are trying to do is to add external users (from an agency partner) to ABP and grant them access to a collection. Counterintuitively, it appears that the way to do this is to create a Product Profile and add users to that Product Profile, and then the Profile shows up like a Group to which a collection can be shared.

I think we’ve just found that “Groups” themselves don’t really do much for us other than basic user segregation since you cannot share a collection with a Group.

If we have that right, then we will just proceed with adding users to the base profile (to ensure they get the email notifying them of their access - which apparently is only triggered from the default profile) and then to a separate  profile  we’ll use to control access to specific collections of assets.

### Example

### How to do

We first create product configurations and then assign users to them.

Admin publishes `assets/folders/collections` from AEM Author to BP (the concept of public folder publish). On BP, Admin can share the `assets/folders/collections` further to other users (Non-admin users like Editors and Viewers). Editors can publish the `assets/folders/collections` further to other users like viewers and editors. But the viewer can only view and not share.

## Why do search suggestions don't come ? {#why-do-search-suggestions-don-t-come}

How Search suggestions work?

Search suggestions for custom properties

Search suggestions only come for...
