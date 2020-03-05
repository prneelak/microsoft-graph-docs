---
title: "List pages"
description: "Get the onenotePages from the pages navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List pages

Namespace: microsoft.graph

Get the onenotePages from the pages navigation property.

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
GET /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onenotePage](../resources/onenotepage.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onenotepage"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onenotepage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 874

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onenotePage",
      "id": "70c2781a-781a-70c2-1a78-c2701a78c270",
      "self": "Self value",
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
      "title": "Title value",
      "createdByAppId": "Created By App Id value",
      "links": {
        "@odata.type": "microsoft.graph.pageLinks",
        "oneNoteClientUrl": {
          "@odata.type": "microsoft.graph.externalLink",
          "href": "Href value"
        },
        "oneNoteWebUrl": {
          "@odata.type": "microsoft.graph.externalLink"
        }
      },
      "contentUrl": "https://example.com/contentUrl/",
      "content": "Stream",
      "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
      "level": 5,
      "order": 5,
      "userTags": [
        "User Tags value"
      ]
    }
  ]
}
```

