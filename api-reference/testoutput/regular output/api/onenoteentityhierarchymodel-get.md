---
title: "Get onenoteEntityHierarchyModel"
description: "Read properties and relationships of the onenoteEntityHierarchyModel object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get onenoteEntityHierarchyModel

Namespace: microsoft.graph

Read properties and relationships of the [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md) object.

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
GET ** Entity URI for microsoft.graph.onenoteEntityHierarchyModel not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onenoteentityhierarchymodel"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.onenoteEntityHierarchyModel not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteEntityHierarchyModel"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 770

{
  "value": {
    "@odata.type": "#microsoft.graph.onenoteEntityHierarchyModel",
    "id": "a7c62a9c-2a9c-a7c6-9c2a-c6a79c2ac6a7",
    "self": "Self value",
    "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
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
    "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00"
  }
}
```

