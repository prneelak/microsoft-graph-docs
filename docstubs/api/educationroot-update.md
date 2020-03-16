---
title: "Update educationRoot"
description: "Update the properties of a educationRoot object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationRoot

Namespace: microsoft.graph

Update the properties of a [educationRoot](../resources/educationroot.md) object.

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
PATCH /education
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [educationRoot](../resources/educationroot.md) object.

The following table shows the properties that are required when you create the [educationRoot](../resources/educationroot.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [educationRoot](../resources/educationroot.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_educationroot"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/education
Content-type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.educationRoot"
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
Content-Length: 104

{
  "@odata.type": "#microsoft.graph.educationRoot",
  "id": "61e047d9-47d9-61e0-d947-e061d947e061"
}
```

