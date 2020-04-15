---
title: "group: assignLicense"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# assignLicense

Namespace: microsoft.graph

**TODO: Add Description**

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /groups/{groupsId}/assignLicense
POST /me/joinedGroups/{groupId}/assignLicense
POST /users/{usersId}/joinedGroups/{groupId}/assignLicense
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|addLicenses|[assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description**|
|removeLicenses|Guid collection|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [group](../resources/group.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/assignLicense

Content-Type: application/json
Content-length: 172

{
  "addLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "removeLicenses": [
    "e3b47097-7097-e3b4-9770-b4e39770b4e3"
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.group",
    "id": "7e5ebbe9-bbe9-7e5e-e9bb-5e7ee9bb5e7e",
    "deletedDateTime": "2016-12-31T23:58:28.3197258+03:00",
    "assignedLabels": [
      {
        "@odata.type": "microsoft.graph.assignedLabel"
      }
    ],
    "assignedLicenses": [
      {
        "@odata.type": "microsoft.graph.assignedLicense"
      }
    ],
    "classification": "Classification value",
    "createdDateTime": "2017-01-01T00:00:27.4994223+03:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "groupTypes": [
      "Group Types value"
    ],
    "hasMembersWithLicenseErrors": true,
    "isAssignableToRole": true,
    "licenseProcessingState": {
      "@odata.type": "microsoft.graph.licenseProcessingState"
    },
    "mail": "Mail value",
    "mailEnabled": true,
    "mailNickname": "Mail Nickname value",
    "mdmAppId": "Mdm App Id value",
    "membershipRule": "Membership Rule value",
    "membershipRuleProcessingState": "Membership Rule Processing State value",
    "onPremisesDomainName": "On Premises Domain Name value",
    "onPremisesLastSyncDateTime": "2016-12-31T23:59:16.9945393+03:00",
    "onPremisesNetBiosName": "On Premises Net Bios Name value",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "microsoft.graph.onPremisesProvisioningError"
      }
    ],
    "onPremisesSamAccountName": "On Premises Sam Account Name value",
    "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
    "onPremisesSyncEnabled": true,
    "preferredDataLocation": "Preferred Data Location value",
    "preferredLanguage": "Preferred Language value",
    "proxyAddresses": [
      "Proxy Addresses value"
    ],
    "renewedDateTime": "2017-01-01T00:02:14.8329799+03:00",
    "resourceBehaviorOptions": [
      "Resource Behavior Options value"
    ],
    "resourceProvisioningOptions": [
      "Resource Provisioning Options value"
    ],
    "securityEnabled": true,
    "securityIdentifier": "Security Identifier value",
    "theme": "Theme value",
    "visibility": "Visibility value",
    "accessType": "String",
    "allowExternalSenders": true,
    "autoSubscribeNewMembers": true,
    "isFavorite": true,
    "isSubscribedByMail": true,
    "unseenCount": 11,
    "unseenConversationsCount": 8,
    "unseenMessagesCount": 3,
    "hideFromOutlookClients": true,
    "hideFromAddressLists": true,
    "isArchived": true
  }
}
```

