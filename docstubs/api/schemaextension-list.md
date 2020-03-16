---
title: "List schemaExtensions"
description: "List properties and relationships of the schemaExtension objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List schemaExtensions

Namespace: microsoft.graph

List properties and relationships of the [schemaExtension](../resources/schemaextension.md) objects.

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
GET /schemaExtensions
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
If successful, this method returns a `200 OK` response code and a collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}
-->
``` http
GET https://graph.microsoft.com/localtest/schemaExtensions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.schemaextension)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 507

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.schemaExtension",
      "id": "9b972427-2427-9b97-2724-979b2724979b",
      "description": "Description value",
      "targetTypes": [
        "Target Types value"
      ],
      "properties": [
        {
          "@odata.type": "microsoft.graph.extensionSchemaProperty",
          "name": "Name value",
          "type": "Type value"
        }
      ],
      "status": "Status value",
      "owner": "Owner value"
    }
  ]
}
```

