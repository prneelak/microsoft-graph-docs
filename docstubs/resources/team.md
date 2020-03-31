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
|[allMessages](../api/team-allmessages.md)|[chatMessage](../resources/chatmessage.md) collection||
|[Get schedule](../api/schedule-get.md)|[schedule](../resources/schedule.md)|Read properties and relationships of the [schedule](../resources/schedule.md) object.|
|[Get group](../api/group-get.md)|[group](../resources/group.md)|Read properties and relationships of the [group](../resources/group.md) object.|
|[Get teamsTemplate](../api/teamstemplate-get.md)|[teamsTemplate](../resources/teamstemplate.md)|Read properties and relationships of the [teamsTemplate](../resources/teamstemplate.md) object.|
|[Get profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilephoto.md)|Read properties and relationships of the [profilePhoto](../resources/profilephoto.md) object.|
|[List owners](../api/team-list-owners.md)|[user](../resources/user.md) collection|Get the users from the owners navigation property.|
|[Create owners](../api/team-post-owners.md)|[user](../resources/user.md)|Create owners by posting to the owners collection.|
|[List channels](../api/team-list-channels.md)|[channel](../resources/channel.md) collection|Get the channels from the channels navigation property.|
|[Add channels](../api/team-post-channels.md)|[channel](../resources/channel.md)|Add channels by posting to the channels collection.|
|[Get channel](../api/channel-get.md)|[channel](../resources/channel.md)|Read properties and relationships of the [channel](../resources/channel.md) object.|
|[List apps](../api/team-list-apps.md)|[teamsCatalogApp](../resources/teamscatalogapp.md) collection|Get the teamsCatalogApps from the apps navigation property.|
|[Add apps](../api/team-post-apps.md)|[teamsCatalogApp](../resources/teamscatalogapp.md)|Add apps by posting to the apps collection.|
|[List installedApps](../api/team-list-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|Get the teamsAppInstallations from the installedApps navigation property.|
|[Add installedApps](../api/team-post-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Add installedApps by posting to the installedApps collection.|
|[List operations](../api/team-list-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md) collection|Get the teamsAsyncOperations from the operations navigation property.|
|[Add operations](../api/team-post-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classification|String||
|description|String||
|discoverySettings|[teamDiscoverySettings](../resources/teamdiscoverysettings.md)||
|displayName|String||
|funSettings|[teamFunSettings](../resources/teamfunsettings.md)||
|guestSettings|[teamGuestSettings](../resources/teamguestsettings.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|internalId|String||
|isArchived|Boolean||
|memberSettings|[teamMemberSettings](../resources/teammembersettings.md)||
|messagingSettings|[teamMessagingSettings](../resources/teammessagingsettings.md)||
|specialization|Enumeration| Possible values are: `none`, `educationStandard`, `educationClass`, `educationProfessionalLearningCommunity`, `educationStaff`, `healthcareStandard`, `healthcareCareCoordination`, `unknownFutureValue`.|
|visibility|Enumeration| Possible values are: `private`, `public`, `hiddenMembership`, `unknownFutureValue`.|
|webUrl|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|apps|[teamsCatalogApp](../resources/teamscatalogapp.md) collection||
|channels|[channel](../resources/channel.md) collection||
|group|[group](../resources/group.md)||
|installedApps|[teamsAppInstallation](../resources/teamsappinstallation.md) collection||
|operations|[teamsAsyncOperation](../resources/teamsasyncoperation.md) collection||
|owners|[user](../resources/user.md) collection||
|photo|[profilePhoto](../resources/profilephoto.md)||
|primaryChannel|[channel](../resources/channel.md)||
|schedule|[schedule](../resources/schedule.md)||
|template|[teamsTemplate](../resources/teamstemplate.md)||

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
  "displayName": "String",
  "description": "String",
  "internalId": "String",
  "classification": "String",
  "specialization": "String",
  "visibility": "String",
  "webUrl": "String",
  "memberSettings": {
    "@odata.type": "microsoft.graph.teamMemberSettings",
    "allowCreateUpdateChannels": true,
    "allowCreatePrivateChannels": true,
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
  "discoverySettings": {
    "@odata.type": "microsoft.graph.teamDiscoverySettings",
    "showInTeamsSearchAndSuggestions": true
  },
  "isArchived": true
}
```

