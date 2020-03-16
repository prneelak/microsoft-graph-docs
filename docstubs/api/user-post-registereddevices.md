---
title: "Create registeredDevices"
description: "Create registeredDevices by posting to the registeredDevices collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create registeredDevices

Namespace: microsoft.graph

Create registeredDevices by posting to the registeredDevices collection.

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
POST /me/registeredDevices/$ref
POST /users/{usersId}/registeredDevices/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [directoryObject](../resources/directoryobject.md) object.

The following table shows the properties that are required when you create the [directoryObject](../resources/directoryobject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryobjects"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/registeredDevices
Content-type: application/json
Content-length: 116

{
  "@odata.type": "#microsoft.graph.directoryObject",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryobject"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 165

{
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "7f4b5789-5789-7f4b-8957-4b7f89574b7f",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00"
}
```

