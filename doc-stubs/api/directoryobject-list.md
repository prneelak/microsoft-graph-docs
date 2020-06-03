---
title: "List directoryObjects"
description: "Get a list of the directoryObject objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List directoryObjects

Namespace: microsoft.graph

Get a list of the [directoryObject](../resources/directoryobject.md) objects and their properties.

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
GET /me/memberOf
GET /me/ownedDevices
GET /me/ownedObjects
GET /directoryObjects
GET /me/directReports
GET /me/createdObjects
GET /stsPolicy/appliesTo
GET /me/registeredDevices
GET /me/transitiveMemberOf
GET /directory/deletedItems
GET /groups/{groupsId}/owners
GET /users/{usersId}/memberOf
GET /groups/{groupsId}/members
GET /groups/{groupsId}/memberOf
GET /devices/{devicesId}/memberOf
GET /users/{usersId}/ownedDevices
GET /users/{usersId}/ownedObjects
GET /users/{usersId}/directReports
GET /contacts/{contactsId}/memberOf
GET /users/{usersId}/createdObjects
GET /users/{usersId}/registeredDevices
GET /users/{usersId}/transitiveMemberOf
GET /contacts/{contactsId}/directReports
GET /devices/{devicesId}/registeredUsers
GET /groups/{groupsId}/transitiveMembers
GET /applications/{applicationsId}/owners
GET /devices/{devicesId}/registeredOwners
GET /groups/{groupsId}/transitiveMemberOf
GET /devices/{devicesId}/transitiveMemberOf
GET /contacts/{contactsId}/transitiveMemberOf
GET /domains/{domainsId}/domainNameReferences
GET /directoryRoles/{directoryRolesId}/members
GET /groups/{groupsId}/membersWithLicenseErrors
GET /servicePrincipals/{servicePrincipalsId}/owners
GET /servicePrincipals/{servicePrincipalsId}/memberOf
GET /administrativeUnits/{administrativeUnitsId}/members
GET /servicePrincipals/{servicePrincipalsId}/ownedObjects
GET /servicePrincipals/{servicePrincipalsId}/createdObjects
GET /servicePrincipals/{servicePrincipalsId}/transitiveMemberOf
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/memberOf
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directoryobject)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directoryObject",
      "id": "f72b1f9d-1f9d-f72b-9d1f-2bf79d1f2bf7",
      "deletedDateTime": "String"
    }
  ]
}
```

