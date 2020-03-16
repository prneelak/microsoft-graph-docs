---
title: "List userStatuses"
description: "Get the deviceConfigurationUserStatuses from the userStatuses navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userStatuses

Namespace: microsoft.graph

Get the deviceConfigurationUserStatuses from the userStatuses navigation property.

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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deviceconfigurationuserstatus"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceconfigurationuserstatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 393

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
      "id": "c6b0ea76-ea76-c6b0-76ea-b0c676eab0c6",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "String",
      "lastReportedDateTime": "2017-01-01T00:00:41.3711013+03:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```

