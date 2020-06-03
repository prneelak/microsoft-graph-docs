---
title: "Create directoryObject"
description: "Create a new directoryObject object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create directoryObject

Namespace: microsoft.graph

Create a new [directoryObject](../resources/directoryobject.md) object.

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
POST /me/memberOf
POST /me/ownedDevices
POST /me/ownedObjects
POST /directoryObjects
POST /me/directReports
POST /me/createdObjects
POST /stsPolicy/appliesTo
POST /me/registeredDevices
POST /me/transitiveMemberOf
POST /directory/deletedItems
POST /groups/{groupsId}/owners
POST /users/{usersId}/memberOf
POST /groups/{groupsId}/members
POST /groups/{groupsId}/memberOf
POST /devices/{devicesId}/memberOf
POST /users/{usersId}/ownedDevices
POST /users/{usersId}/ownedObjects
POST /users/{usersId}/directReports
POST /contacts/{contactsId}/memberOf
POST /users/{usersId}/createdObjects
POST /users/{usersId}/registeredDevices
POST /users/{usersId}/transitiveMemberOf
POST /contacts/{contactsId}/directReports
POST /devices/{devicesId}/registeredUsers
POST /groups/{groupsId}/transitiveMembers
POST /applications/{applicationsId}/owners
POST /devices/{devicesId}/registeredOwners
POST /groups/{groupsId}/transitiveMemberOf
POST /devices/{devicesId}/transitiveMemberOf
POST /contacts/{contactsId}/transitiveMemberOf
POST /domains/{domainsId}/domainNameReferences
POST /directoryRoles/{directoryRolesId}/members
POST /groups/{groupsId}/membersWithLicenseErrors
POST /servicePrincipals/{servicePrincipalsId}/owners
POST /servicePrincipals/{servicePrincipalsId}/memberOf
POST /administrativeUnits/{administrativeUnitsId}/members
POST /servicePrincipals/{servicePrincipalsId}/ownedObjects
POST /servicePrincipals/{servicePrincipalsId}/createdObjects
POST /servicePrincipals/{servicePrincipalsId}/transitiveMemberOf
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [directoryObject](../resources/directoryobject.md) object.

The following table shows the properties that are required when you create the [directoryObject](../resources/directoryobject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryobjects"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/memberOf
Content-Type: application/json
Content-length: 89

{
  "@odata.type": "#microsoft.graph.directoryObject",
  "deletedDateTime": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryobject"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "f72b1f9d-1f9d-f72b-9d1f-2bf79d1f2bf7",
  "deletedDateTime": "String"
}
```

