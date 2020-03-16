---
title: "checkin"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# checkin

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
POST /me/drive/root/checkin
POST /drives/{drivesId}/root/checkin
POST /shares/{sharesId}/root/checkin
POST /workbooks/{workbooksId}/checkin
POST /shares/{sharesId}/driveItem/checkin
POST /me/drive/items/{driveItemId}/checkin
POST /me/drive/special/{driveItemId}/checkin
POST /drives/{drivesId}/items/{driveItemId}/checkin
POST /shares/{sharesId}/items/{driveItemId}/checkin
POST /drives/{drivesId}/special/{driveItemId}/checkin
POST /workbooks/{workbooksId}/children/{driveItemId}/checkin
POST /me/drive/items/{driveItemId}/listItem/driveItem/checkin
POST /me/drive/items/{driveItemId}/children/{driveItemId}/checkin
POST /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/checkin
POST /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/checkin
POST /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/checkin
POST /me/drive/items/{driveItemId}/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/checkin
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|checkInAs|String||
|comment|String||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "driveitem_checkin"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/root/checkin

Content-type: application/json
Content-length: 71

{
  "checkInAs": "Check In As value",
  "comment": "Comment value"
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
HTTP/1.1 204 No Content
```

