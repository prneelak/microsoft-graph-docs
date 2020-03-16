---
title: "Update auditLogRoot"
description: "Update the properties of a auditLogRoot object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update auditLogRoot

Namespace: microsoft.graph

Update the properties of a [auditLogRoot](../resources/auditlogroot.md) object.

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
PATCH /auditLogs
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [auditLogRoot](../resources/auditlogroot.md) object.

The following table shows the properties that are required when you create the [auditLogRoot](../resources/auditlogroot.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [auditLogRoot](../resources/auditlogroot.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_auditlogroot"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/auditLogs
Content-type: application/json
Content-length: 54

{
  "@odata.type": "#microsoft.graph.auditLogRoot"
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
Content-Length: 103

{
  "@odata.type": "#microsoft.graph.auditLogRoot",
  "id": "c73f2472-2472-c73f-7224-3fc772243fc7"
}
```

