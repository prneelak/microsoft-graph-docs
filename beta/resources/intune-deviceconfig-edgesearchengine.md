---
title: "edgeSearchEngine resource type"
description: "Allows IT admins to set a predefined default search engine for MDM-Controlled devices."
author: "davidmu1"
localization_priority: Normal
ms.prod: "Intune"
doc_type: resourcePageType
---

# edgeSearchEngine resource type

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Allows IT admins to set a predefined default search engine for MDM-Controlled devices.


Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|edgeSearchEngineType|[edgeSearchEngineType](../resources/intune-deviceconfig-edgesearchenginetype.md)|Allows IT admins to set a predefined default search engine for MDM-Controlled devices. Possible values are: `default`, `bing`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```



