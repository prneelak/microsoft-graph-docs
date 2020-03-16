---
title: "Get mobileApp"
description: "Read properties and relationships of the mobileApp object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get mobileApp

Namespace: microsoft.graph

Read properties and relationships of the [mobileApp](../resources/mobileapp.md) object.

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
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [mobileApp](../resources/mobileapp.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mobileapp"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceAppManagement/mobileApps/{mobileAppId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 799

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileApp",
    "id": "18243925-3925-1824-2539-241825392418",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
    "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "publishingState": "String"
  }
}
```

