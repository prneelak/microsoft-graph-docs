---
title: "apiApplication resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# apiApplication resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptMappedClaims|Boolean||
|knownClientApplications|Guid collection||
|oauth2PermissionScopes|[permissionScope](../resources/permissionscope.md) collection||
|preAuthorizedApplications|[preAuthorizedApplication](../resources/preauthorizedapplication.md) collection||
|requestedAccessTokenVersion|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.apiApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.apiApplication",
  "acceptMappedClaims": true,
  "knownClientApplications": [
    "Guid"
  ],
  "preAuthorizedApplications": [
    {
      "@odata.type": "microsoft.graph.preAuthorizedApplication",
      "appId": "String",
      "delegatedPermissionIds": [
        "String"
      ]
    }
  ],
  "requestedAccessTokenVersion": 1024,
  "oauth2PermissionScopes": [
    {
      "@odata.type": "microsoft.graph.permissionScope",
      "adminConsentDescription": "String",
      "adminConsentDisplayName": "String",
      "id": "Guid",
      "isEnabled": true,
      "origin": "String",
      "type": "String",
      "userConsentDescription": "String",
      "userConsentDisplayName": "String",
      "value": "String"
    }
  ]
}
```

