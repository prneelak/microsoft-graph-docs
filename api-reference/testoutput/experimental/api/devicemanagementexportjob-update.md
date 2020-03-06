---
title: "Update deviceManagementExportJob"
description: "Update the properties of a deviceManagementExportJob object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementExportJob

Namespace: microsoft.graph

Update the properties of a [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.

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
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.

The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/devicemanagementexportjob.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportName|String|Name of the report|
|filter|String|Filters applied on the report|
|select|String collection|Columns selected from the report|
|format|Enumeration|Format of the exported report. Possible values are: `csv`, `pdf`.|
|snapshotId|String|A snapshot is an identifiable subset of the dataset represented by the ReportName. A sessionId or CachedReportConfiguration id can be used here. If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId. Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.|
|status|Enumeration|Status of the export job. Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|String|Temporary location of the exported report|
|requestDateTime|DateTimeOffset|Time that the exported report was requested|
|expirationDateTime|DateTimeOffset|Time that the exported report expires|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementexportjob"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
Content-type: application/json
Content-length: 403

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "String",
  "snapshotId": "Snapshot Id value",
  "status": "String",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:11.7450092+03:00",
  "expirationDateTime": "2017-01-01T00:01:27.2282595+03:00"
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
Content-Length: 452

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "32006966-6966-3200-6669-003266690032",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "String",
  "snapshotId": "Snapshot Id value",
  "status": "String",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:11.7450092+03:00",
  "expirationDateTime": "2017-01-01T00:01:27.2282595+03:00"
}
```

