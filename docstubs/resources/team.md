---
title: "team resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# team resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List teams](../api/team-list.md)|[team](../resources/team.md) collection|List properties and relationships of the [team](../resources/team.md) objects.|
|[Get team](../api/team-get.md)|[team](../resources/team.md)|Read properties and relationships of the [team](../resources/team.md) object.|
|[Create team](../api/team-post-teams.md)|[team](../resources/team.md)|Create a new [team](../resources/team.md) object.|
|[Delete team](../api/team-delete.md)|None|Deletes a [team](../resources/team.md).|
|[Update team](../api/team-update.md)|[team](../resources/team.md)|Update the properties of a [team](../resources/team.md) object.|
|[clone](../api/team-clone.md)|None||
|[archive](../api/team-archive.md)|None||
|[unarchive](../api/team-unarchive.md)|None||
|[List channels](../api/team-list-channels.md)|[channel](../resources/channel.md) collection|Get the channels from the channels navigation property.|
|[Add channels](../api/team-post-channels.md)|[channel](../resources/channel.md)|Add channels by posting to the channels collection.|
|[List installedApps](../api/team-list-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|Get the teamsAppInstallations from the installedApps navigation property.|
|[Add installedApps](../api/team-post-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Add installedApps by posting to the installedApps collection.|
|[List operations](../api/team-list-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md) collection|Get the teamsAsyncOperations from the operations navigation property.|
|[Add operations](../api/team-post-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|funSettings|[teamFunSettings](../resources/teamfunsettings.md)||
|guestSettings|[teamGuestSettings](../resources/teamguestsettings.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|isArchived|Boolean||
|memberSettings|[teamMemberSettings](../resources/teammembersettings.md)||
|messagingSettings|[teamMessagingSettings](../resources/teammessagingsettings.md)||
|webUrl|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|channels|[channel](../resources/channel.md) collection||
|installedApps|[teamsAppInstallation](../resources/teamsappinstallation.md) collection||
|operations|[teamsAsyncOperation](../resources/teamsasyncoperation.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.team",
  "id": "String (identifier)",
  "webUrl": "String",
  "memberSettings": {
    "@odata.type": "microsoft.graph.teamMemberSettings",
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true
  },
  "guestSettings": {
    "@odata.type": "microsoft.graph.teamGuestSettings"
  },
  "messagingSettings": {
    "@odata.type": "microsoft.graph.teamMessagingSettings",
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true
  },
  "funSettings": {
    "@odata.type": "microsoft.graph.teamFunSettings",
    "allowGiphy": true,
    "giphyContentRating": "String",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  },
  "isArchived": true
}
```

