---
title: "auditLogRoot resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# auditLogRoot resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get auditLogRoot](../api/auditlogroot-get.md)|[auditLogRoot](../resources/auditlogroot.md)|Read properties and relationships of the [auditLogRoot](../resources/auditlogroot.md) object.|
|[Update auditLogRoot](../api/auditlogroot-update.md)|[auditLogRoot](../resources/auditlogroot.md)|Update the properties of a [auditLogRoot](../resources/auditlogroot.md) object.|
|[List signIns](../api/auditlogroot-list-signins.md)|[signIn](../resources/signin.md) collection|Get the signIns from the signIns navigation property.|
|[Add signIns](../api/auditlogroot-post-signins.md)|[signIn](../resources/signin.md)|Add signIns by posting to the signIns collection.|
|[List directoryAudits](../api/auditlogroot-list-directoryaudits.md)|[directoryAudit](../resources/directoryaudit.md) collection|Get the directoryAudits from the directoryAudits navigation property.|
|[Add directoryAudits](../api/auditlogroot-post-directoryaudits.md)|[directoryAudit](../resources/directoryaudit.md)|Add directoryAudits by posting to the directoryAudits collection.|
|[List restrictedSignIns](../api/auditlogroot-list-restrictedsignins.md)|[restrictedSignIn](../resources/restrictedsignin.md) collection|Get the restrictedSignIns from the restrictedSignIns navigation property.|
|[Add restrictedSignIns](../api/auditlogroot-post-restrictedsignins.md)|[restrictedSignIn](../resources/restrictedsignin.md)|Add restrictedSignIns by posting to the restrictedSignIns collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|directoryAudits|[directoryAudit](../resources/directoryaudit.md) collection||
|restrictedSignIns|[restrictedSignIn](../resources/restrictedsignin.md) collection||
|signIns|[signIn](../resources/signin.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditLogRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditLogRoot",
  "id": "String (identifier)"
}
```

