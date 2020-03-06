---
title: "Update deviceAppManagementTask"
description: "Update the properties of a deviceAppManagementTask object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceAppManagementTask

Namespace: microsoft.graph

Update the properties of a [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object.

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
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object.

The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/deviceappmanagementtask.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The name.|
|description|String|The description.|
|createdDateTime|DateTimeOffset|The created date.|
|dueDateTime|DateTimeOffset|The due date.|
|category|Enumeration|The category. Possible values are: `unknown`, `advancedThreatProtection`.|
|priority|Enumeration|The priority. Possible values are: `none`, `high`, `low`.|
|creator|String|The email address of the creator.|
|creatorNotes|String|Notes from the creator.|
|assignedTo|String|The name or email of the admin this task is assigned to.|
|status|Enumeration|The status. Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_deviceappmanagementtask"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
Content-type: application/json
Content-length: 381

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2016-12-31T23:58:39.04111+03:00",
  "category": "String",
  "priority": "String",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "String"
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
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "9351bccf-bccf-9351-cfbc-5193cfbc5193",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "dueDateTime": "2016-12-31T23:58:39.04111+03:00",
  "category": "String",
  "priority": "String",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "String"
}
```

