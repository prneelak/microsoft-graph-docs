---
title: "Create schemaExtension"
description: "Create a new schemaExtension object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create schemaExtension

Namespace: microsoft.graph

Create a new [schemaExtension](../resources/schemaextension.md) object.

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
POST /schemaExtensions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [schemaExtension](../resources/schemaextension.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions"
}
-->
``` http
POST https://graph.microsoft.com/localtest/schemaExtensions
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
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaextension"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 414

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
```

