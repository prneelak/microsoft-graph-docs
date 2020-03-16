---
title: "auditActivityInitiator resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# auditActivityInitiator resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|app|[appIdentity](../resources/appidentity.md)||
|user|[userIdentity](../resources/useridentity.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActivityInitiator",
  "user": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "String",
    "displayName": "String",
    "ipAddress": "String",
    "userPrincipalName": "String"
  },
  "app": {
    "@odata.type": "microsoft.graph.appIdentity",
    "appId": "String",
    "servicePrincipalId": "String",
    "servicePrincipalName": "String"
  }
}
```

