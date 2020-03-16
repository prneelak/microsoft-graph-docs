---
title: "Update dataPolicyOperation"
description: "Update the properties of a dataPolicyOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update dataPolicyOperation

Namespace: microsoft.graph

Update the properties of a [dataPolicyOperation](../resources/datapolicyoperation.md) object.

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
PATCH /dataPolicyOperations/{dataPolicyOperationsId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [dataPolicyOperation](../resources/datapolicyoperation.md) object.

The following table shows the properties that are required when you create the [dataPolicyOperation](../resources/datapolicyoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|completedDateTime|DateTimeOffset||
|status|Enumeration|. Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|String||
|userId|String||
|submittedDateTime|DateTimeOffset||
|progress|Double||



## Response
If successful, this method returns a `200 OK` response code and an updated [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_datapolicyoperation"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/dataPolicyOperations/{dataPolicyOperationsId}
Content-type: application/json
Content-length: 309

{
  "@odata.type": "#microsoft.graph.dataPolicyOperation",
  "completedDateTime": "2017-01-01T00:01:15.9862985+03:00",
  "status": "String",
  "storageLocation": "Storage Location value",
  "userId": "User Id value",
  "submittedDateTime": "2016-12-31T23:59:32.7259666+03:00",
  "progress": "Double"
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
Content-Length: 358

{
  "@odata.type": "#microsoft.graph.dataPolicyOperation",
  "id": "c61b40b8-40b8-c61b-b840-1bc6b8401bc6",
  "completedDateTime": "2017-01-01T00:01:15.9862985+03:00",
  "status": "String",
  "storageLocation": "Storage Location value",
  "userId": "User Id value",
  "submittedDateTime": "2016-12-31T23:59:32.7259666+03:00",
  "progress": "Double"
}
```

