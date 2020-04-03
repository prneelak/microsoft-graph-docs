---
title: "Get outlookTask"
description: "Read properties and relationships of the outlookTask object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get outlookTask

Namespace: microsoft.graph

Read properties and relationships of the [outlookTask](../resources/outlooktask.md) object.

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
GET /me/outlook/tasks/{outlookTaskId}
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/outlook/tasks/{outlookTaskId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1879

{
  "value": {
    "@odata.type": "#microsoft.graph.outlookTask",
    "id": "eb4db4f5-b4f5-eb4d-f5b4-4debf5b44deb",
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "assignedTo": "Assigned To value",
    "body": {
      "@odata.type": "microsoft.graph.itemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "completedDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "Date Time value",
      "timeZone": "Time Zone value"
    },
    "dueDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "hasAttachments": true,
    "importance": "String",
    "isReminderOn": true,
    "owner": "Owner value",
    "parentFolderId": "Parent Folder Id value",
    "recurrence": {
      "@odata.type": "microsoft.graph.patternedRecurrence",
      "pattern": {
        "@odata.type": "microsoft.graph.recurrencePattern",
        "type": "String",
        "interval": 8,
        "month": 5,
        "dayOfMonth": 10,
        "daysOfWeek": [
          "String"
        ],
        "firstDayOfWeek": "String",
        "index": "String"
      },
      "range": {
        "@odata.type": "microsoft.graph.recurrenceRange",
        "type": "String",
        "startDate": "Date",
        "endDate": "Date",
        "recurrenceTimeZone": "Recurrence Time Zone value",
        "numberOfOccurrences": 3
      }
    },
    "reminderDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "sensitivity": "String",
    "startDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "status": "String",
    "subject": "Subject value"
  }
}
```

