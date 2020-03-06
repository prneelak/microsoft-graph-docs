---
title: "Update deviceManagementReportSchedule"
description: "Update the properties of a deviceManagementReportSchedule object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementReportSchedule

Namespace: microsoft.graph

Update the properties of a [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.

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
PATCH /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.

The following table shows the properties that are required when you create the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportScheduleName|String|Name of the schedule|
|subject|String|Subject of the scheduled reports that are delivered|
|emails|String collection|Emails to which the scheduled reports are delivered|
|recurrence|Enumeration|Frequency of scheduled report delivery. Possible values are: `none`, `daily`, `weekly`, `monthly`.|
|startDateTime|DateTimeOffset|Time that the delivery of the scheduled reports starts|
|endDateTime|DateTimeOffset|Time that the delivery of the scheduled reports ends|
|userId|String|The Id of the User who created the report|
|reportName|String|Name of the report|
|filter|String|Filters applied on the report|
|select|String collection|Columns selected from the report|
|orderBy|String collection|Ordering of columns in the report|
|format|Enumeration|Format of the scheduled report. Possible values are: `csv`, `pdf`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementreportschedule"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
Content-type: application/json
Content-length: 542

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
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
Content-Length: 591

{
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
```

