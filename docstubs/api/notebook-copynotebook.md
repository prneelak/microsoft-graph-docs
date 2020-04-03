---
title: "copyNotebook"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# copyNotebook

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
POST /me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/copyNotebook
POST /me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentNotebook/copyNotebook
POST /me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/parentNotebook/copyNotebook
POST /me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}/parentNotebook/copyNotebook
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|groupId|String||
|renameAs|String||
|notebookFolder|String||
|siteCollectionId|String||
|siteId|String||



## Response
If successful, this action returns a `200 OK` response code and a [onenoteOperation](../resources/onenoteoperation.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/copyNotebook

Content-type: application/json
Content-length: 196

{
  "groupId": "Group Id value",
  "renameAs": "Rename As value",
  "notebookFolder": "Notebook Folder value",
  "siteCollectionId": "Site Collection Id value",
  "siteId": "Site Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteoperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "value": {
    "@odata.type": "#microsoft.graph.onenoteOperation",
    "id": "6adaeffd-effd-6ada-fdef-da6afdefda6a",
    "status": "String",
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
    "lastActionDateTime": "2016-12-31T23:58:25.2668755+00:00",
    "resourceLocation": "Resource Location value",
    "resourceId": "Resource Id value",
    "error": {
      "@odata.type": "microsoft.graph.onenoteOperationError"
    },
    "percentComplete": "Percent Complete value"
  }
}
```

