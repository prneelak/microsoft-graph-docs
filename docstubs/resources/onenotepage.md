---
title: "onenotePage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onenotePage resource type


Namespace: microsoft.graph




Inherits from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onenotePage](../api/onenotepage-get.md)|[onenotePage](../resources/onenotepage.md)|Read properties and relationships of the [onenotePage](../resources/onenotepage.md) object.|
|[Update onenotePage](../api/onenotepage-update.md)|[onenotePage](../resources/onenotepage.md)|Update the properties of a [onenotePage](../resources/onenotepage.md) object.|
|[onenotePatchContent](../api/onenotepage-onenotepatchcontent.md)|None||
|[preview](../api/onenotepage-preview.md)|[onenotePagePreview](../resources/onenotepagepreview.md)||
|[copyToSection](../api/onenotepage-copytosection.md)|[onenoteOperation](../resources/onenoteoperation.md)||
|[Get onenoteSection](../api/onenotesection-get.md)|[onenoteSection](../resources/onenotesection.md)|Read properties and relationships of the [onenoteSection](../resources/onenotesection.md) object.|
|[Get notebook](../api/notebook-get.md)|[notebook](../resources/notebook.md)|Read properties and relationships of the [notebook](../resources/notebook.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Stream||
|contentUrl|String||
|createdByAppId|String||
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|level|Int32||
|links|[pageLinks](../resources/pagelinks.md)||
|order|Int32||
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|title|String||
|userTags|String collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|parentNotebook|[notebook](../resources/notebook.md)||
|parentSection|[onenoteSection](../resources/onenotesection.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenotePage",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenotePage",
  "id": "String (identifier)",
  "self": "String",
  "createdDateTime": "String (timestamp)",
  "title": "String",
  "createdByAppId": "String",
  "links": {
    "@odata.type": "microsoft.graph.pageLinks"
  },
  "contentUrl": "String",
  "content": "Stream",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "order": 1024,
  "userTags": [
    "String"
  ]
}
```

