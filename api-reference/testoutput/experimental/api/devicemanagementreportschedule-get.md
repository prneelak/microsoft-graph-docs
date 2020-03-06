---
title: "Get deviceManagementReportSchedule"
description: "Read properties and relationships of the deviceManagementReportSchedule object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceManagementReportSchedule

Namespace: microsoft.graph

Read properties and relationships of the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.

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
GET /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
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
If successful, this method returns a `200 OK` response code and [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementreportschedule"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementReportSchedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 650

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
    "id": "b0c44614-4614-b0c4-1446-c4b01446c4b0",
    "reportScheduleName": "Report Schedule Name value",
    "subject": "Subject value",
    "emails": [
      "Emails value"
    ],
    "recurrence": "String",
    "startDateTime": "2017-01-01T00:00:14.2767228+03:00",
    "endDateTime": "2017-01-01T00:02:18.392989+03:00",
    "userId": "User Id value",
    "reportName": "Report Name value",
    "filter": "Filter value",
    "select": [
      "Select value"
    ],
    "orderBy": [
      "Order By value"
    ],
    "format": "String"
  }
}
```

