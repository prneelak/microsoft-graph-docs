---
title: "Get sectionGroup"
description: "Read properties and relationships of the sectionGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get sectionGroup

Namespace: microsoft.graph

Read properties and relationships of the [sectionGroup](../resources/sectiongroup.md) object.

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
GET /me/onenote/sectionGroups/{sectionGroupId}
GET /me/onenote/notebooks/{notebookId}/sectionGroups/{sectionGroupId}
GET /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup
GET /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/parentSectionGroup
GET /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/sectionGroups/{sectionGroupId}
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
If successful, this method returns a `200 OK` response code and [sectionGroup](../resources/sectiongroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/onenote/sectionGroups/{sectionGroupId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 879

{
  "value": {
    "@odata.type": "#microsoft.graph.sectionGroup",
    "id": "9c856a38-6a38-9c85-386a-859c386a859c",
    "self": "Self value",
    "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
    "displayName": "Display Name value",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
    "sectionsUrl": "https://example.com/sectionsUrl/",
    "sectionGroupsUrl": "https://example.com/sectionGroupsUrl/"
  }
}
```

