---
title: "Add managedEBooks"
description: "Add managedEBooks by posting to the managedEBooks collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add managedEBooks

Namespace: microsoft.graph

Add managedEBooks by posting to the managedEBooks collection.

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
POST /deviceAppManagement/managedEBooks/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedEBook](../resources/managedebook.md) object.

The following table shows the properties that are required when you create the [managedEBook](../resources/managedebook.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Name of the eBook.|
|description|String|Description.|
|publisher|String|Publisher.|
|publishedDateTime|DateTimeOffset|The date and time when the eBook was published.|
|largeCover|[mimeContent](../resources/mimecontent.md)|Book cover.|
|createdDateTime|DateTimeOffset|The date and time when the eBook file was created.|
|lastModifiedDateTime|DateTimeOffset|The date and time when the eBook was last modified.|
|informationUrl|String|The more information Url.|
|privacyInformationUrl|String|The privacy statement Url.|



## Response
If successful, this method returns a `201 Created` response code and a [managedEBook](../resources/managedebook.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managedebook_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 491

{
  "@odata.type": "#microsoft.graph.managedEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:56:39.4901133+03:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedebook"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 663

{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "73db37a8-37a8-73db-a837-db73a837db73",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:56:39.4901133+03:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
}
```

