---
title: "Update managedAppOperation"
description: "Update the properties of a managedAppOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update managedAppOperation

Namespace: microsoft.graph

Update the properties of a [managedAppOperation](../resources/managedappoperation.md) object.

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
PATCH /me/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [managedAppOperation](../resources/managedappoperation.md) object.

The following table shows the properties that are required when you create the [managedAppOperation](../resources/managedappoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The operation name.|
|lastModifiedDateTime|DateTimeOffset|The last time the app operation was modified.|
|state|String|The current state of the operation|
|version|String|Version of the entity.|



## Response
If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/managedappoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_managedappoperation"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
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
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "id": "a683f191-f191-a683-91f1-83a691f183a6",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "state": "State value",
  "version": "Version value"
}
```

