---
title: "Update schemaExtension"
description: "Update the properties of a schemaExtension object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update schemaExtension

Namespace: microsoft.graph

Update the properties of a [schemaExtension](../resources/schemaextension.md) object.

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
PATCH /schemaExtensions/{schemaExtensionsId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [schemaExtension](../resources/schemaextension.md) object.

The following table shows the properties that are required when you create the [schemaExtension](../resources/schemaextension.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String||
|targetTypes|String collection||
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection||
|status|String||
|owner|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [schemaExtension](../resources/schemaextension.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/schemaExtensions/{schemaExtensionsId}
Content-type: application/json
Content-length: 365

{
  "@odata.type": "#microsoft.graph.schemaExtension",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 414

{
  "@odata.type": "#microsoft.graph.schemaExtension",
  "id": "12dbf903-f903-12db-03f9-db1203f9db12",
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
```

