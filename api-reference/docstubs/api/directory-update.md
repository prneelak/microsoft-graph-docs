---
title: "Update directory"
description: "Update the properties of a directory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update directory

Namespace: microsoft.graph

Update the properties of a [directory](../resources/directory.md) object.

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
PATCH /directory
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [directory](../resources/directory.md) object.

The following table shows the properties that are required when you create the [directory](../resources/directory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [directory](../resources/directory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_directory"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory
Content-type: application/json
Content-length: 51

{
  "@odata.type": "#microsoft.graph.directory"
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
Content-Length: 100

{
  "@odata.type": "#microsoft.graph.directory",
  "id": "f5a63e68-3e68-f5a6-683e-a6f5683ea6f5"
}
```

