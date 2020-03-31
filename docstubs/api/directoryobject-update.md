---
title: "Update directoryObject"
description: "Update the properties of a directoryObject object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update directoryObject

Namespace: microsoft.graph

Update the properties of a [directoryObject](../resources/directoryobject.md) object.

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
PATCH /directoryObjects/{directoryObjectsId}
PATCH /directory/deletedItems/{directoryObjectId}
PATCH /groups/{groupsId}/acceptedSenders/{directoryObjectId}
PATCH /groups/{groupsId}/rejectedSenders/{directoryObjectId}
PATCH /me/joinedGroups/{groupId}/acceptedSenders/{directoryObjectId}
PATCH /me/joinedGroups/{groupId}/rejectedSenders/{directoryObjectId}
PATCH /directory/featureRolloutPolicies/{featureRolloutPolicyId}/appliesTo/{directoryObjectId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [directoryObject](../resources/directoryobject.md) object.

The following table shows the properties that are required when you create the [directoryObject](../resources/directoryobject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_directoryobject"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directoryObjects/{directoryObjectsId}
Content-type: application/json
Content-length: 116

{
  "@odata.type": "#microsoft.graph.directoryObject",
  "deletedDateTime": "2017-01-01T00:02:56.4302403+03:00"
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
Content-Length: 165

{
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "9bd39918-9918-9bd3-1899-d39b1899d39b",
  "deletedDateTime": "2017-01-01T00:02:56.4302403+03:00"
}
```

