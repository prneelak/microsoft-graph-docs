---
title: "vpnProxyServer resource type"
description: "VPN Proxy Server."
author: "davidmu1"
localization_priority: Normal
ms.prod: "Intune"
doc_type: resourcePageType
---

# vpnProxyServer resource type

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

VPN Proxy Server.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|automaticConfigurationScriptUrl|String|Proxy's automatic configuration script url.|
|address|String|Address.|
|port|Int32|Port. Valid values 0 to 65535|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```



