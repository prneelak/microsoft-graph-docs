---
title: "Update group"
description: "Update the properties of a group object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update group

Namespace: microsoft.graph

Update the properties of a [group](../resources/group.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /groups/{groupsId}
PATCH /me/joinedTeams/{groupId}
PATCH /users/{usersId}/joinedTeams/{groupId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [group](../resources/group.md) object.

The following table shows the properties that are required when you create the [group](../resources/group.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection||
|classification|String||
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|hasMembersWithLicenseErrors|Boolean||
|groupTypes|String collection||
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
|visibility|String||
|allowExternalSenders|Boolean||
|autoSubscribeNewMembers|Boolean||
|isSubscribedByMail|Boolean||
|unseenCount|Int32||
|isArchived|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [group](../resources/group.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_group"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/groups/{groupsId}
Content-type: application/json
Content-length: 1913

{
  "@odata.type": "#microsoft.graph.group",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "9f014a7b-4a7b-9f01-7b4a-019f7b4a019f"
      ],
      "skuId": "5fc5df95-df95-5fc5-95df-c55f95dfc55f"
    }
  ],
  "classification": "Classification value",
  "description": "Description value",
  "displayName": "Display Name value",
  "hasMembersWithLicenseErrors": true,
  "groupTypes": [
    "Group Types value"
  ],
  "licenseProcessingState": {
    "@odata.type": "microsoft.graph.licenseProcessingState",
    "state": "State value"
  },
  "mail": "Mail value",
  "mailEnabled": true,
  "mailNickname": "Mail Nickname value",
  "onPremisesDomainName": "On Premises Domain Name value",
  "onPremisesLastSyncDateTime": "2017-01-01T00:03:13.2795175+03:00",
  "onPremisesNetBiosName": "On Premises Net Bios Name value",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:56:37.8106884+03:00"
    }
  ],
  "onPremisesSamAccountName": "On Premises Sam Account Name value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "Preferred Data Location value",
  "proxyAddresses": [
    "Proxy Addresses value"
  ],
  "renewedDateTime": "2016-12-31T23:58:39.4846964+03:00",
  "securityEnabled": true,
  "securityIdentifier": "Security Identifier value",
  "visibility": "Visibility value",
  "allowExternalSenders": true,
  "autoSubscribeNewMembers": true,
  "isSubscribedByMail": true,
  "unseenCount": 11,
  "isArchived": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2021

{
  "@odata.type": "#microsoft.graph.group",
  "id": "f3f112a8-12a8-f3f1-a812-f1f3a812f1f3",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "9f014a7b-4a7b-9f01-7b4a-019f7b4a019f"
      ],
      "skuId": "5fc5df95-df95-5fc5-95df-c55f95dfc55f"
    }
  ],
  "classification": "Classification value",
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "hasMembersWithLicenseErrors": true,
  "groupTypes": [
    "Group Types value"
  ],
  "licenseProcessingState": {
    "@odata.type": "microsoft.graph.licenseProcessingState",
    "state": "State value"
  },
  "mail": "Mail value",
  "mailEnabled": true,
  "mailNickname": "Mail Nickname value",
  "onPremisesDomainName": "On Premises Domain Name value",
  "onPremisesLastSyncDateTime": "2017-01-01T00:03:13.2795175+03:00",
  "onPremisesNetBiosName": "On Premises Net Bios Name value",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:56:37.8106884+03:00"
    }
  ],
  "onPremisesSamAccountName": "On Premises Sam Account Name value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "Preferred Data Location value",
  "proxyAddresses": [
    "Proxy Addresses value"
  ],
  "renewedDateTime": "2016-12-31T23:58:39.4846964+03:00",
  "securityEnabled": true,
  "securityIdentifier": "Security Identifier value",
  "visibility": "Visibility value",
  "allowExternalSenders": true,
  "autoSubscribeNewMembers": true,
  "isSubscribedByMail": true,
  "unseenCount": 11,
  "isArchived": true
}
```

