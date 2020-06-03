---
title: "Update directoryObject"
description: "Update the properties of a directoryObject object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update directoryObject

Namespace: microsoft.graph

Update the properties of a [directoryObject](../resources/directoryobject.md) object.

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
PATCH /me/manager
PATCH /users/{usersId}/manager
PATCH /contacts/{contactsId}/manager
PATCH /me/memberOf/{directoryObjectId}
PATCH /groups/{groupsId}/createdOnBehalfOf
PATCH /me/ownedDevices/{directoryObjectId}
PATCH /me/ownedObjects/{directoryObjectId}
PATCH /me/directReports/{directoryObjectId}
PATCH /directoryObjects/{directoryObjectsId}
PATCH /me/createdObjects/{directoryObjectId}
PATCH /stsPolicy/appliesTo/{directoryObjectId}
PATCH /me/registeredDevices/{directoryObjectId}
PATCH /me/transitiveMemberOf/{directoryObjectId}
PATCH /directory/deletedItems/{directoryObjectId}
PATCH /applications/{applicationsId}/createdOnBehalfOf
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

If successful, this method returns a `200 OK` response code and an updated [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_directoryobject"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/manager
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "f72b1f9d-1f9d-f72b-9d1f-2bf79d1f2bf7",
  "deletedDateTime": "String"
}
```

