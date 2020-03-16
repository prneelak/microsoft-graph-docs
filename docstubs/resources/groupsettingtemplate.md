---
title: "groupSettingTemplate resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupSettingTemplate resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupSettingTemplates](../api/groupsettingtemplate-list.md)|[groupSettingTemplate](../resources/groupsettingtemplate.md) collection|List properties and relationships of the [groupSettingTemplate](../resources/groupsettingtemplate.md) objects.|
|[Get groupSettingTemplate](../api/groupsettingtemplate-get.md)|[groupSettingTemplate](../resources/groupsettingtemplate.md)|Read properties and relationships of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object.|
|[Create groupSettingTemplate](../api/groupsettingtemplate-post-groupsettingtemplates.md)|[groupSettingTemplate](../resources/groupsettingtemplate.md)|Create a new [groupSettingTemplate](../resources/groupsettingtemplate.md) object.|
|[Delete groupSettingTemplate](../api/groupsettingtemplate-delete.md)|None|Deletes a [groupSettingTemplate](../resources/groupsettingtemplate.md).|
|[Update groupSettingTemplate](../api/groupsettingtemplate-update.md)|[groupSettingTemplate](../resources/groupsettingtemplate.md)|Update the properties of a [groupSettingTemplate](../resources/groupsettingtemplate.md) object.|
|[checkMemberGroups](../api/groupsettingtemplate-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/groupsettingtemplate-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/groupsettingtemplate-getmembergroups.md)|String collection||
|[getMemberObjects](../api/groupsettingtemplate-getmemberobjects.md)|String collection||
|[restore](../api/groupsettingtemplate-restore.md)|[directoryObject](../resources/directoryobject.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|values|[settingTemplateValue](../resources/settingtemplatevalue.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupSettingTemplate",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingTemplateValue"
    }
  ]
}
```

