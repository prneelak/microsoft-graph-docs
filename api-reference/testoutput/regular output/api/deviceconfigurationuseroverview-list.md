---
title: "List deviceConfigurationUserOverviews"
description: "List properties and relationships of the deviceConfigurationUserOverview objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceConfigurationUserOverviews

Namespace: microsoft.graph

List properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) objects.

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
GET ** Collection URI for microsoft.graph.deviceConfigurationUserOverview not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deviceconfigurationuseroverview"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.deviceConfigurationUserOverview not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceconfigurationuseroverview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
      "id": "559b930c-930c-559b-0c93-9b550c939b55",
      "pendingCount": 12,
      "notApplicableCount": 2,
      "successCount": 12,
      "errorCount": 10,
      "failedCount": 11,
      "lastUpdateDateTime": "2017-01-01T00:03:07.1140227+03:00",
      "configurationVersion": 4
    }
  ]
}
```

