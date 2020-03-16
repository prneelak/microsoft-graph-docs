---
title: "driveItemVersion resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# driveItemVersion resource type


Namespace: microsoft.graph




Inherits from [baseItemVersion](../resources/baseitemversion.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get driveItemVersion](../api/driveitemversion-get.md)|[driveItemVersion](../resources/driveitemversion.md)|Read properties and relationships of the [driveItemVersion](../resources/driveitemversion.md) object.|
|[Update driveItemVersion](../api/driveitemversion-update.md)|[driveItemVersion](../resources/driveitemversion.md)|Update the properties of a [driveItemVersion](../resources/driveitemversion.md) object.|
|[restoreVersion](../api/driveitemversion-restoreversion.md)|None||
|[List versions](../api/driveitem-list-versions.md)|[driveItemVersion](../resources/driveitemversion.md) collection|Get the driveItemVersions from the versions navigation property.|
|[Add versions](../api/driveitem-post-versions.md)|[driveItemVersion](../resources/driveitemversion.md)|Add versions by posting to the versions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Stream||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|publication|[publicationFacet](../resources/publicationfacet.md)| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|size|Int64||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "baseType": "microsoft.graph.baseItemVersion",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.driveItemVersion",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "content": "Stream",
  "size": 1024
}
```

