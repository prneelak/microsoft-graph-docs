---
title: "deviceManagementReports: getCachedReport"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getCachedReport

Namespace: microsoft.graph

**TODO: Add Description**

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCachedReport
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|select|String collection|**TODO: Add Description**|
|search|String|**TODO: Add Description**|
|groupBy|String collection|**TODO: Add Description**|
|orderBy|String collection|**TODO: Add Description**|
|skip|Int32|**TODO: Add Description**|
|top|Int32|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a Stream in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "devicemanagementreports_getcachedreport"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getCachedReport

Content-Type: application/json
Content-length: 195

{
  "id": "String",
  "select": [
    "String"
  ],
  "search": "String",
  "groupBy": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "skip": "Integer",
  "top": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "edm.stream"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": "Stream"
}
```

