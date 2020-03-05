---
title: "getNotebookFromWebUrl"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getNotebookFromWebUrl

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
POST /me/onenote/notebooks/getNotebookFromWebUrl
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|webUrl|String||



## Response
If successful, this action returns a `200 OK` response code and a [CopyNotebookModel](../resources/copynotebookmodel.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "notebook_getnotebookfromweburl"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/onenote/notebooks/getNotebookFromWebUrl

Content-type: application/json
Content-length: 47

{
  "webUrl": "https://example.com/webUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.copynotebookmodel"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": {
    "@odata.type": "microsoft.graph.CopyNotebookModel"
  }
}
```

