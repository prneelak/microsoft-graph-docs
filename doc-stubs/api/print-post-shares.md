---
title: "Create shares"
description: "Create a new shares object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create shares

Namespace: microsoft.graph

Create a new shares object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [printerShare](../resources/printershare.md) object.

The following table shows the properties that are required when you create the [printerShare](../resources/printershare.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|manufacturer|String|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|model|String|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|isAcceptingJobs|Boolean|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|defaults|[printerDefaults](../resources/printerdefaults.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|location|[printerLocation](../resources/printerlocation.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|capabilities|[printerCapabilities](../resources/printercapabilities.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|status|[printerStatus](../resources/printerstatus.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/shares
Content-Type: application/json
Content-length: 471

{
  "@odata.type": "#microsoft.graph.printerShare",
  "name": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printershare"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.printerShare",
  "id": "1c31be74-be74-1c31-74be-311c74be311c",
  "name": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  },
  "createdDateTime": "String (timestamp)"
}
```

