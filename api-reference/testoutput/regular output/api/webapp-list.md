---
title: "List webApps"
description: "List properties and relationships of the webApp objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List webApps

Namespace: microsoft.graph

List properties and relationships of the [webApp](../resources/webapp.md) objects.

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
GET ** Collection URI for microsoft.graph.webApp not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [webApp](../resources/webapp.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_webapp"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.webApp not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.webapp)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 928

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.webApp",
      "id": "49273614-3614-4927-1436-274914362749",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
      "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "publishingState": "String",
      "appUrl": "https://example.com/appUrl/",
      "useManagedBrowser": true
    }
  ]
}
```

