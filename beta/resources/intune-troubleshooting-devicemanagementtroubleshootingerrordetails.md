---
title: "deviceManagementTroubleshootingErrorDetails resource type"
description: "Object containing detailed information about the error and its remediation."
author: "davidmu1"
localization_priority: Normal
ms.prod: "Intune"
doc_type: resourcePageType
---

# deviceManagementTroubleshootingErrorDetails resource type

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Object containing detailed information about the error and its remediation.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|context|String|Not yet documented|
|failure|String|Not yet documented|
|failureDetails|String|The detailed description of what went wrong.|
|remediation|String|The detailed description of how to remediate this issue.|
|resources|[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection|Links to helpful documentation about this failure.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```



