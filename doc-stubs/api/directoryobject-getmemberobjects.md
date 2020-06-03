---
title: "directoryObject: getMemberObjects"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getMemberObjects

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
POST /me/manager/getMemberObjects
POST /users/{usersId}/manager/getMemberObjects
POST /contacts/{contactsId}/manager/getMemberObjects
POST /me/memberOf/{directoryObjectId}/getMemberObjects
POST /groups/{groupsId}/createdOnBehalfOf/getMemberObjects
POST /me/ownedDevices/{directoryObjectId}/getMemberObjects
POST /me/ownedObjects/{directoryObjectId}/getMemberObjects
POST /me/directReports/{directoryObjectId}/getMemberObjects
POST /directoryObjects/{directoryObjectsId}/getMemberObjects
POST /me/createdObjects/{directoryObjectId}/getMemberObjects
POST /stsPolicy/appliesTo/{directoryObjectId}/getMemberObjects
POST /me/registeredDevices/{directoryObjectId}/getMemberObjects
POST /me/transitiveMemberOf/{directoryObjectId}/getMemberObjects
POST /directory/deletedItems/{directoryObjectId}/getMemberObjects
POST /applications/{applicationsId}/createdOnBehalfOf/getMemberObjects
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|securityEnabledOnly|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a String collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/manager/getMemberObjects

Content-Type: application/json
Content-length: 39

{
  "securityEnabledOnly": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(edm.string)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    "String"
  ]
}
```

