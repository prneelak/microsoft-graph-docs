---
title: "userTeamwork resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userTeamwork resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List userTeamworks](../api/userteamwork-list.md)|[userTeamwork](../resources/userteamwork.md) collection|Get a list of the [userTeamwork](../resources/userteamwork.md) objects and their properties.|
|[Create userTeamwork](../api/userteamwork-create.md)|[userTeamwork](../resources/userteamwork.md)|Create a new [userTeamwork](../resources/userteamwork.md) object.|
|[Get userTeamwork](../api/userteamwork-get.md)|[userTeamwork](../resources/userteamwork.md)|Read the properties and relationships of a [userTeamwork](../resources/userteamwork.md) object.|
|[Update userTeamwork](../api/userteamwork-update.md)|[userTeamwork](../resources/userteamwork.md)|Update the properties of a [userTeamwork](../resources/userteamwork.md) object.|
|[Delete userTeamwork](../api/userteamwork-delete.md)|None|Deletes a [userTeamwork](../resources/userteamwork.md) object.|
|[sendActivityNotification](../api/userteamwork-sendactivitynotification.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|installedApps|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userTeamwork",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userTeamwork",
  "id": "String (identifier)"
}
```

