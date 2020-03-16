---
title: "Get deviceComplianceDeviceOverview"
description: "Read properties and relationships of the deviceComplianceDeviceOverview object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceComplianceDeviceOverview

Namespace: microsoft.graph

Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.

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
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
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
If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicecompliancedeviceoverview"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 367

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
    "id": "9b826a16-6a16-9b82-166a-829b166a829b",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:59:58.1382181+03:00",
    "configurationVersion": 4
  }
}
```

