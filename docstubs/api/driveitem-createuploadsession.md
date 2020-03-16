---
title: "createUploadSession"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# createUploadSession

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
POST /me/drive/root/createUploadSession
POST /drives/{drivesId}/root/createUploadSession
POST /shares/{sharesId}/root/createUploadSession
POST /workbooks/{workbooksId}/createUploadSession
POST /shares/{sharesId}/driveItem/createUploadSession
POST /me/drive/items/{driveItemId}/createUploadSession
POST /me/drive/special/{driveItemId}/createUploadSession
POST /drives/{drivesId}/items/{driveItemId}/createUploadSession
POST /shares/{sharesId}/items/{driveItemId}/createUploadSession
POST /drives/{drivesId}/special/{driveItemId}/createUploadSession
POST /workbooks/{workbooksId}/children/{driveItemId}/createUploadSession
POST /me/drive/items/{driveItemId}/listItem/driveItem/createUploadSession
POST /me/drive/items/{driveItemId}/children/{driveItemId}/createUploadSession
POST /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/createUploadSession
POST /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/createUploadSession
POST /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/createUploadSession
POST /me/drive/items/{driveItemId}/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/createUploadSession
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
|item|[driveItemUploadableProperties](../resources/driveitemuploadableproperties.md)||



## Response
If successful, this action returns a `200 OK` response code and a [uploadSession](../resources/uploadsession.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "driveitem_createuploadsession"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/root/createUploadSession

Content-type: application/json
Content-length: 90

{
  "item": {
    "@odata.type": "microsoft.graph.driveItemUploadableProperties"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadsession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 75

{
  "value": {
    "@odata.type": "microsoft.graph.uploadSession"
  }
}
```

