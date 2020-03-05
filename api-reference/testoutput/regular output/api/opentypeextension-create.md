---
title: "Create openTypeExtension"
description: "Create a new openTypeExtension object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create openTypeExtension

Namespace: microsoft.graph

Create a new [openTypeExtension](../resources/opentypeextension.md) object.

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
POST ** Collection URI for microsoft.graph.openTypeExtension not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [openTypeExtension](../resources/opentypeextension.md) object.

The following table shows the properties that are required when you create the [openTypeExtension](../resources/opentypeextension.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|extensionName|String||



## Response
If successful, this method returns a `201 Created` response code and a [openTypeExtension](../resources/opentypeextension.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_opentypeextension_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.openTypeExtension not found
Content-type: application/json
Content-length: 103

{
  "@odata.type": "#microsoft.graph.openTypeExtension",
  "extensionName": "Extension Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.opentypeextension"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 152

{
  "@odata.type": "#microsoft.graph.openTypeExtension",
  "id": "4db1c125-c125-4db1-25c1-b14d25c1b14d",
  "extensionName": "Extension Name value"
}
```

