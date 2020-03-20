---
title: "List groups"
description: "List properties and relationships of the group objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List groups

Namespace: microsoft.graph

List properties and relationships of the [group](../resources/group.md) objects.

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
GET /groups
GET /me/joinedTeams
GET /users/{usersId}/joinedTeams
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groups
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.group)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "ff0bcf1d-cf1d-ff0b-1dcf-0bff1dcf0bff",
      "deletedDateTime": "2017-01-01T00:02:30.3038128+03:00",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense",
          "disabledPlans": [
            "e2540f5d-0f5d-e254-5d0f-54e25d0f54e2"
          ],
          "skuId": "77d817ab-17ab-77d8-ab17-d877ab17d877"
        }
      ],
      "classification": "Classification value",
      "createdDateTime": "2016-12-31T23:59:21.2140811+03:00",
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
      "onPremisesLastSyncDateTime": "2017-01-01T00:00:46.2905907+03:00",
      "onPremisesNetBiosName": "On Premises Net Bios Name value",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2016-12-31T23:57:53.9463324+03:00"
        }
      ],
      "onPremisesSamAccountName": "On Premises Sam Account Name value",
      "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
      "onPremisesSyncEnabled": true,
      "preferredDataLocation": "Preferred Data Location value",
      "proxyAddresses": [
        "Proxy Addresses value"
      ],
      "renewedDateTime": "2016-12-31T23:58:19.838817+03:00",
      "securityEnabled": true,
      "securityIdentifier": "Security Identifier value",
      "visibility": "Visibility value",
      "allowExternalSenders": true,
      "autoSubscribeNewMembers": true,
      "isSubscribedByMail": true,
      "unseenCount": 11,
      "isArchived": true
    }
  ]
}
```

