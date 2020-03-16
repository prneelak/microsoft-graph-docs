---
title: "security resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# security resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get security](../api/security-get.md)|[security](../resources/security.md)|Read properties and relationships of the [security](../resources/security.md) object.|
|[Update security](../api/security-update.md)|[security](../resources/security.md)|Update the properties of a [security](../resources/security.md) object.|
|[List alerts](../api/security-list-alerts.md)|[alert](../resources/alert.md) collection|Get the alerts from the alerts navigation property.|
|[Add alerts](../api/security-post-alerts.md)|[alert](../resources/alert.md)|Add alerts by posting to the alerts collection.|
|[List secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md) collection|Get the secureScoreControlProfiles from the secureScoreControlProfiles navigation property.|
|[Add secureScoreControlProfiles](../api/security-post-securescorecontrolprofiles.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md)|Add secureScoreControlProfiles by posting to the secureScoreControlProfiles collection.|
|[List secureScores](../api/security-list-securescores.md)|[secureScore](../resources/securescore.md) collection|Get the secureScores from the secureScores navigation property.|
|[Add secureScores](../api/security-post-securescores.md)|[secureScore](../resources/securescore.md)|Add secureScores by posting to the secureScores collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|alerts|[alert](../resources/alert.md) collection||
|secureScoreControlProfiles|[secureScoreControlProfile](../resources/securescorecontrolprofile.md) collection||
|secureScores|[secureScore](../resources/securescore.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security",
  "id": "String (identifier)"
}
```

