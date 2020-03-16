---
title: "Get mobileThreatDefenseConnector"
description: "Read properties and relationships of the mobileThreatDefenseConnector object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get mobileThreatDefenseConnector

Namespace: microsoft.graph

Read properties and relationships of the [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.

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
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
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
If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mobilethreatdefenseconnector"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileThreatDefenseConnector"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 498

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
    "id": "4648427c-427c-4648-7c42-48467c424846",
    "lastHeartbeatDateTime": "2016-12-31T23:58:49.272366+03:00",
    "partnerState": "String",
    "androidEnabled": true,
    "iosEnabled": true,
    "androidDeviceBlockedOnMissingPartnerData": true,
    "iosDeviceBlockedOnMissingPartnerData": true,
    "partnerUnsupportedOsVersionBlocked": true,
    "partnerUnresponsivenessThresholdInDays": 6
  }
}
```

