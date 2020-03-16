---
title: "groupSetting resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupSetting resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupSettings](../api/groupsetting-list.md)|[groupSetting](../resources/groupsetting.md) collection|List properties and relationships of the [groupSetting](../resources/groupsetting.md) objects.|
|[Get groupSetting](../api/groupsetting-get.md)|[groupSetting](../resources/groupsetting.md)|Read properties and relationships of the [groupSetting](../resources/groupsetting.md) object.|
|[Create groupSetting](../api/groupsetting-post-groupsettings.md)|[groupSetting](../resources/groupsetting.md)|Create a new [groupSetting](../resources/groupsetting.md) object.|
|[Delete groupSetting](../api/groupsetting-delete.md)|None|Deletes a [groupSetting](../resources/groupsetting.md).|
|[Update groupSetting](../api/groupsetting-update.md)|[groupSetting](../resources/groupsetting.md)|Update the properties of a [groupSetting](../resources/groupsetting.md) object.|
|[List settings](../api/group-list-settings.md)|[groupSetting](../resources/groupsetting.md) collection|Get the groupSettings from the settings navigation property.|
|[Add settings](../api/group-post-settings.md)|[groupSetting](../resources/groupsetting.md)|Add settings by posting to the settings collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|templateId|String||
|values|[settingValue](../resources/settingvalue.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupSetting",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupSetting",
  "id": "String (identifier)",
  "displayName": "String",
  "templateId": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingValue"
    }
  ]
}
```

