---
title: "groupLifecyclePolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupLifecyclePolicy resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupLifecyclePolicies](../api/grouplifecyclepolicy-list.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) collection|List properties and relationships of the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects.|
|[Get groupLifecyclePolicy](../api/grouplifecyclepolicy-get.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Read properties and relationships of the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.|
|[Create groupLifecyclePolicy](../api/grouplifecyclepolicy-post-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Create a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.|
|[Delete groupLifecyclePolicy](../api/grouplifecyclepolicy-delete.md)|None|Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).|
|[Update groupLifecyclePolicy](../api/grouplifecyclepolicy-update.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Update the properties of a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.|
|[addGroup](../api/grouplifecyclepolicy-addgroup.md)|Boolean||
|[removeGroup](../api/grouplifecyclepolicy-removegroup.md)|Boolean||
|[List groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) collection|Get the groupLifecyclePolicies from the groupLifecyclePolicies navigation property.|
|[Add groupLifecyclePolicies](../api/group-post-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Add groupLifecyclePolicies by posting to the groupLifecyclePolicies collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alternateNotificationEmails|String||
|groupLifetimeInDays|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|managedGroupTypes|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupLifecyclePolicy",
  "id": "String (identifier)",
  "groupLifetimeInDays": 1024,
  "managedGroupTypes": "String",
  "alternateNotificationEmails": "String"
}
```

