---
title: "contactFolder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# contactFolder resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get contactFolder](../api/contactfolder-get.md)|[contactFolder](../resources/contactfolder.md)|Read properties and relationships of the [contactFolder](../resources/contactfolder.md) object.|
|[Update contactFolder](../api/contactfolder-update.md)|[contactFolder](../resources/contactfolder.md)|Update the properties of a [contactFolder](../resources/contactfolder.md) object.|
|[delta](../api/contactfolder-delta.md)|[contactFolder](../resources/contactfolder.md) collection||
|[List singleValueExtendedProperties](../api/contactfolder-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/contactfolder-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/contactfolder-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/contactfolder-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List contacts](../api/contactfolder-list-contacts.md)|[contact](../resources/contact.md) collection|Get the contacts from the contacts navigation property.|
|[Add contacts](../api/contactfolder-post-contacts.md)|[contact](../resources/contact.md)|Add contacts by posting to the contacts collection.|
|[List childFolders](../api/contactfolder-list-childfolders.md)|[contactFolder](../resources/contactfolder.md) collection|Get the contactFolders from the childFolders navigation property.|
|[Add childFolders](../api/contactfolder-post-childfolders.md)|[contactFolder](../resources/contactfolder.md)|Add childFolders by posting to the childFolders collection.|
|[List childFolders](../api/contactfolder-list-childfolders.md)|[contactFolder](../resources/contactfolder.md) collection|Get the contactFolders from the childFolders navigation property.|
|[Add childFolders](../api/contactfolder-post-childfolders.md)|[contactFolder](../resources/contactfolder.md)|Add childFolders by posting to the childFolders collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|parentFolderId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|childFolders|[contactFolder](../resources/contactfolder.md) collection||
|contacts|[contact](../resources/contact.md) collection||
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection||
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contactFolder",
  "id": "String (identifier)",
  "parentFolderId": "String",
  "displayName": "String"
}
```

