---
title: "directoryObject: getMemberGroups"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getMemberGroups

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
POST /me/manager/getMemberGroups
POST /users/{usersId}/manager/getMemberGroups
POST /contacts/{contactsId}/manager/getMemberGroups
POST /me/memberOf/{directoryObjectId}/getMemberGroups
POST /groups/{groupsId}/createdOnBehalfOf/getMemberGroups
POST /me/ownedDevices/{directoryObjectId}/getMemberGroups
POST /me/ownedObjects/{directoryObjectId}/getMemberGroups
POST /me/directReports/{directoryObjectId}/getMemberGroups
POST /directoryObjects/{directoryObjectsId}/getMemberGroups
POST /me/createdObjects/{directoryObjectId}/getMemberGroups
POST /stsPolicy/appliesTo/{directoryObjectId}/getMemberGroups
POST /me/registeredDevices/{directoryObjectId}/getMemberGroups
POST /me/transitiveMemberOf/{directoryObjectId}/getMemberGroups
POST /directory/deletedItems/{directoryObjectId}/getMemberGroups
POST /applications/{applicationsId}/createdOnBehalfOf/getMemberGroups
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this action returns a `200 OK` response code and a Boolean collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/manager/getMemberGroups
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(edm.boolean)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    "Boolean"
  ]
}
```

