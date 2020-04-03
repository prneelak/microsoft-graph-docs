---
title: "browserSyncSetting enum type"
description: "Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings. Option to prevent syncing across devices, but allow user override."
author: "davidmu1"
localization_priority: Normal
ms.prod: "Intune"
doc_type: enumPageType
---

# browserSyncSetting enum type

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings. Option to prevent syncing across devices, but allow user override.

## Members
|Member|Value|Description|
|:---|:---|:---|
|notConfigured|0|Default – Allow syncing of browser settings across devices.|
|blockedWithUserOverride|1|Prevent syncing of browser settings across user devices, allow user override of setting.|
|blocked|2|Absolutely prevent syncing of browser settings across user devices.|



