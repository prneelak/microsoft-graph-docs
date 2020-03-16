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
GET /me/drive/root/getActivitiesByInterval
GET /drives/{drivesId}/root/getActivitiesByInterval
GET /shares/{sharesId}/root/getActivitiesByInterval
GET /workbooks/{workbooksId}/getActivitiesByInterval
GET /shares/{sharesId}/driveItem/getActivitiesByInterval
GET /me/drive/items/{driveItemId}/getActivitiesByInterval
GET /me/drive/special/{driveItemId}/getActivitiesByInterval
GET /drives/{drivesId}/items/{driveItemId}/getActivitiesByInterval
GET /shares/{sharesId}/items/{driveItemId}/getActivitiesByInterval
GET /drives/{drivesId}/special/{driveItemId}/getActivitiesByInterval
GET /workbooks/{workbooksId}/children/{driveItemId}/getActivitiesByInterval
GET /me/drive/items/{driveItemId}/listItem/driveItem/getActivitiesByInterval
GET /me/drive/items/{driveItemId}/children/{driveItemId}/getActivitiesByInterval
GET /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/getActivitiesByInterval
GET /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/getActivitiesByInterval
GET /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/getActivitiesByInterval
GET /me/drive/items/{driveItemId}/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/getActivitiesByInterval
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
  "name": "driveitem_getactivitiesbyinterval"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/root/getActivitiesByInterval
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

