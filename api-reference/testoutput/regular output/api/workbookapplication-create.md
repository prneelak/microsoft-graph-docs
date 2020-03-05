---
title: "Create workbookApplication"
description: "Create a new workbookApplication object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookApplication

Namespace: microsoft.graph

Create a new [workbookApplication](../resources/workbookapplication.md) object.

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
POST ** Collection URI for microsoft.graph.workbookApplication not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookApplication](../resources/workbookapplication.md) object.

The following table shows the properties that are required when you create the [workbookApplication](../resources/workbookapplication.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|calculationMode|String||



## Response
If successful, this method returns a `201 Created` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookapplication_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookApplication not found
Content-type: application/json
Content-length: 109

{
  "@odata.type": "#microsoft.graph.workbookApplication",
  "calculationMode": "Calculation Mode value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookapplication"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 158

{
  "@odata.type": "#microsoft.graph.workbookApplication",
  "id": "8d09a040-a040-8d09-40a0-098d40a0098d",
  "calculationMode": "Calculation Mode value"
}
```

