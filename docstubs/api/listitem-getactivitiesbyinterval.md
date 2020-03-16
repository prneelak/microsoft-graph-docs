---
title: "getActivitiesByInterval"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getActivitiesByInterval

Namespace: microsoft.graph



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
GET /shares/{sharesId}/listItem/getActivitiesByInterval
GET /me/drive/list/items/{listItemId}/getActivitiesByInterval
GET /workbooks/{workbooksId}/listItem/getActivitiesByInterval
GET /me/drive/items/{driveItemId}/listItem/getActivitiesByInterval
GET /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/listItem/getActivitiesByInterval
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [itemActivityStat](../resources/itemactivitystat.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "listitem_getactivitiesbyinterval"
}
-->
``` http
GET https://graph.microsoft.com/localtest/shares/{sharesId}/listItem/getActivitiesByInterval
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemactivitystat)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 815

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.itemActivityStat",
      "id": "5a0c294c-294c-5a0c-4c29-0c5a4c290c5a",
      "startDateTime": "2017-01-01T00:02:40.1232988+03:00",
      "endDateTime": "2017-01-01T00:02:20.5434752+03:00",
      "access": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "create": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "delete": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "edit": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "move": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "isTrending": true,
      "incompleteData": {
        "@odata.type": "microsoft.graph.incompleteData"
      }
    }
  ]
}
```

