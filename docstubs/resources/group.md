---
title: "group resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# group resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groups](../api/group-list.md)|[group](../resources/group.md) collection|List properties and relationships of the [group](../resources/group.md) objects.|
|[Get group](../api/group-get.md)|[group](../resources/group.md)|Read properties and relationships of the [group](../resources/group.md) object.|
|[Create group](../api/group-post-groups.md)|[group](../resources/group.md)|Create a new [group](../resources/group.md) object.|
|[Delete group](../api/group-delete.md)|None|Deletes a [group](../resources/group.md).|
|[Update group](../api/group-update.md)|[group](../resources/group.md)|Update the properties of a [group](../resources/group.md) object.|
|[delta](../api/group-delta.md)|[group](../resources/group.md) collection||
|[checkMemberGroups](../api/group-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/group-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/group-getmembergroups.md)|String collection||
|[getMemberObjects](../api/group-getmemberobjects.md)|String collection||
|[restore](../api/group-restore.md)|[directoryObject](../resources/directoryobject.md)||
|[validateProperties](../api/group-validateproperties.md)|None||
|[subscribeByMail](../api/group-subscribebymail.md)|None||
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|None||
|[addFavorite](../api/group-addfavorite.md)|None||
|[removeFavorite](../api/group-removefavorite.md)|None||
|[resetUnseenCount](../api/group-resetunseencount.md)|None||
|[renew](../api/group-renew.md)|None||
|[List members](../api/group-list-members.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the members navigation property.|
|[Create members](../api/group-post-members.md)|[directoryObject](../resources/directoryobject.md)|Create members by posting to the members collection.|
|[List memberOf](../api/group-list-memberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Create memberOf](../api/group-post-memberof.md)|[directoryObject](../resources/directoryobject.md)|Create memberOf by posting to the memberOf collection.|
|[List membersWithLicenseErrors](../api/group-list-memberswithlicenseerrors.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the membersWithLicenseErrors navigation property.|
|[Create membersWithLicenseErrors](../api/group-post-memberswithlicenseerrors.md)|[directoryObject](../resources/directoryobject.md)|Create membersWithLicenseErrors by posting to the membersWithLicenseErrors collection.|
|[List transitiveMembers](../api/group-list-transitivemembers.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMembers navigation property.|
|[Create transitiveMembers](../api/group-post-transitivemembers.md)|[directoryObject](../resources/directoryobject.md)|Create transitiveMembers by posting to the transitiveMembers collection.|
|[List transitiveMemberOf](../api/group-list-transitivememberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Create transitiveMemberOf](../api/group-post-transitivememberof.md)|[directoryObject](../resources/directoryobject.md)|Create transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryobject.md)|Read properties and relationships of the [directoryObject](../resources/directoryobject.md) object.|
|[List owners](../api/group-list-owners.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the owners navigation property.|
|[Create owners](../api/group-post-owners.md)|[directoryObject](../resources/directoryobject.md)|Create owners by posting to the owners collection.|
|[List settings](../api/group-list-settings.md)|[groupSetting](../resources/groupsetting.md) collection|Get the groupSettings from the settings navigation property.|
|[Add settings](../api/group-post-settings.md)|[groupSetting](../resources/groupsetting.md)|Add settings by posting to the settings collection.|
|[List conversations](../api/group-list-conversations.md)|[conversation](../resources/conversation.md) collection|Get the conversations from the conversations navigation property.|
|[Add conversations](../api/group-post-conversations.md)|[conversation](../resources/conversation.md)|Add conversations by posting to the conversations collection.|
|[List photos](../api/group-list-photos.md)|[profilePhoto](../resources/profilephoto.md) collection|Get the profilePhotos from the photos navigation property.|
|[Add photos](../api/group-post-photos.md)|[profilePhoto](../resources/profilephoto.md)|Add photos by posting to the photos collection.|
|[List acceptedSenders](../api/group-list-acceptedsenders.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the acceptedSenders navigation property.|
|[Add acceptedSenders](../api/group-post-acceptedsenders.md)|[directoryObject](../resources/directoryobject.md)|Add acceptedSenders by posting to the acceptedSenders collection.|
|[List rejectedSenders](../api/group-list-rejectedsenders.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the rejectedSenders navigation property.|
|[Add rejectedSenders](../api/group-post-rejectedsenders.md)|[directoryObject](../resources/directoryobject.md)|Add rejectedSenders by posting to the rejectedSenders collection.|
|[List threads](../api/group-list-threads.md)|[conversationThread](../resources/conversationthread.md) collection|Get the conversationThreads from the threads navigation property.|
|[Add threads](../api/group-post-threads.md)|[conversationThread](../resources/conversationthread.md)|Add threads by posting to the threads collection.|
|[Get calendar](../api/calendar-get.md)|[calendar](../resources/calendar.md)|Read properties and relationships of the [calendar](../resources/calendar.md) object.|
|[List calendarView](../api/group-list-calendarview.md)|[event](../resources/event.md) collection|Get the events from the calendarView navigation property.|
|[Add calendarView](../api/group-post-calendarview.md)|[event](../resources/event.md)|Add calendarView by posting to the calendarView collection.|
|[List events](../api/group-list-events.md)|[event](../resources/event.md) collection|Get the events from the events navigation property.|
|[Add events](../api/group-post-events.md)|[event](../resources/event.md)|Add events by posting to the events collection.|
|[Get profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilephoto.md)|Read properties and relationships of the [profilePhoto](../resources/profilephoto.md) object.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read properties and relationships of the [drive](../resources/drive.md) object.|
|[List drives](../api/group-list-drives.md)|[drive](../resources/drive.md) collection|Get the drives from the drives navigation property.|
|[Add drives](../api/group-post-drives.md)|[drive](../resources/drive.md)|Add drives by posting to the drives collection.|
|[List sites](../api/group-list-sites.md)|[site](../resources/site.md) collection|Get the sites from the sites navigation property.|
|[Add sites](../api/group-post-sites.md)|[site](../resources/site.md)|Add sites by posting to the sites collection.|
|[List extensions](../api/group-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/group-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|
|[List groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) collection|Get the groupLifecyclePolicies from the groupLifecyclePolicies navigation property.|
|[Add groupLifecyclePolicies](../api/group-post-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Add groupLifecyclePolicies by posting to the groupLifecyclePolicies collection.|
|[Get plannerGroup](../api/plannergroup-get.md)|[plannerGroup](../resources/plannergroup.md)|Read properties and relationships of the [plannerGroup](../resources/plannergroup.md) object.|
|[Get onenote](../api/onenote-get.md)|[onenote](../resources/onenote.md)|Read properties and relationships of the [onenote](../resources/onenote.md) object.|
|[Get team](../api/team-get.md)|[team](../resources/team.md)|Read properties and relationships of the [team](../resources/team.md) object.|
|[List joinedTeams](../api/user-list-joinedteams.md)|[group](../resources/group.md) collection|Get the groups from the joinedTeams navigation property.|
|[Add joinedTeams](../api/user-post-joinedteams.md)|[group](../resources/group.md)|Add joinedTeams by posting to the joinedTeams collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowExternalSenders|Boolean||
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection||
|autoSubscribeNewMembers|Boolean||
|classification|String||
|createdDateTime|DateTimeOffset||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String||
|displayName|String||
|groupTypes|String collection||
|hasMembersWithLicenseErrors|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|isArchived|Boolean||
|isSubscribedByMail|Boolean||
|licenseProcessingState|[licenseProcessingState](../resources/licenseprocessingstate.md)||
|mail|String||
|mailEnabled|Boolean||
|mailNickname|String||
|onPremisesDomainName|String||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesNetBiosName|String||
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection||
|onPremisesSamAccountName|String||
|onPremisesSecurityIdentifier|String||
|onPremisesSyncEnabled|Boolean||
|preferredDataLocation|String||
|proxyAddresses|String collection||
|renewedDateTime|DateTimeOffset||
|securityEnabled|Boolean||
|securityIdentifier|String||
|unseenCount|Int32||
|visibility|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|acceptedSenders|[directoryObject](../resources/directoryobject.md) collection||
|calendar|[calendar](../resources/calendar.md)||
|calendarView|[event](../resources/event.md) collection||
|conversations|[conversation](../resources/conversation.md) collection||
|createdOnBehalfOf|[directoryObject](../resources/directoryobject.md)||
|drive|[drive](../resources/drive.md)||
|drives|[drive](../resources/drive.md) collection||
|events|[event](../resources/event.md) collection||
|extensions|[extension](../resources/extension.md) collection||
|groupLifecyclePolicies|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) collection||
|memberOf|[directoryObject](../resources/directoryobject.md) collection||
|members|[directoryObject](../resources/directoryobject.md) collection||
|membersWithLicenseErrors|[directoryObject](../resources/directoryobject.md) collection||
|onenote|[onenote](../resources/onenote.md)||
|owners|[directoryObject](../resources/directoryobject.md) collection||
|photo|[profilePhoto](../resources/profilephoto.md)||
|photos|[profilePhoto](../resources/profilephoto.md) collection||
|planner|[plannerGroup](../resources/plannergroup.md)||
|rejectedSenders|[directoryObject](../resources/directoryobject.md) collection||
|settings|[groupSetting](../resources/groupsetting.md) collection||
|sites|[site](../resources/site.md) collection||
|team|[team](../resources/team.md)||
|threads|[conversationThread](../resources/conversationthread.md) collection||
|transitiveMemberOf|[directoryObject](../resources/directoryobject.md) collection||
|transitiveMembers|[directoryObject](../resources/directoryobject.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.group",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "Guid"
      ],
      "skuId": "Guid"
    }
  ],
  "classification": "String",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "hasMembersWithLicenseErrors": true,
  "groupTypes": [
    "String"
  ],
  "licenseProcessingState": {
    "@odata.type": "microsoft.graph.licenseProcessingState",
    "state": "String"
  },
  "mail": "String",
  "mailEnabled": true,
  "mailNickname": "String",
  "onPremisesDomainName": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesNetBiosName": "String",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "String",
      "category": "String",
      "propertyCausingError": "String",
      "occurredDateTime": "String (timestamp)"
    }
  ],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "String",
  "proxyAddresses": [
    "String"
  ],
  "renewedDateTime": "String (timestamp)",
  "securityEnabled": true,
  "securityIdentifier": "String",
  "visibility": "String",
  "allowExternalSenders": true,
  "autoSubscribeNewMembers": true,
  "isSubscribedByMail": true,
  "unseenCount": 1024,
  "isArchived": true
}
```

