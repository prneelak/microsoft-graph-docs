---
title: "listItemVersion resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# listItemVersion resource type


Namespace: microsoft.graph




Inherits from [baseItemVersion](../resources/baseitemversion.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get listItemVersion](../api/listitemversion-get.md)|[listItemVersion](../resources/listitemversion.md)|Read properties and relationships of the [listItemVersion](../resources/listitemversion.md) object.|
|[Update listItemVersion](../api/listitemversion-update.md)|[listItemVersion](../resources/listitemversion.md)|Update the properties of a [listItemVersion](../resources/listitemversion.md) object.|
|[restoreVersion](../api/listitemversion-restoreversion.md)|None||
|[Get fieldValueSet](../api/fieldvalueset-get.md)|[fieldValueSet](../resources/fieldvalueset.md)|Read properties and relationships of the [fieldValueSet](../resources/fieldvalueset.md) object.|
|[List versions](../api/listitem-list-versions.md)|[listItemVersion](../resources/listitemversion.md) collection|Get the listItemVersions from the versions navigation property.|
|[Add versions](../api/listitem-post-versions.md)|[listItemVersion](../resources/listitemversion.md)|Add versions by posting to the versions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|publication|[publicationFacet](../resources/publicationfacet.md)| Inherited from [baseItemVersion](../resources/baseitemversion.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fields|[fieldValueSet](../resources/fieldvalueset.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.listItemVersion",
  "baseType": "microsoft.graph.baseItemVersion",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.listItemVersion",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "String",
      "id": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "String",
    "versionId": "String"
  }
}
```

