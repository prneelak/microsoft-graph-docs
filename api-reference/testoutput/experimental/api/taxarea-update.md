---
title: "Update taxArea"
description: "Update the properties of a taxArea object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update taxArea

Namespace: microsoft.graph

Update the properties of a [taxArea](../resources/taxarea.md) object.

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
PATCH /financials/companies/{companyId}/taxAreas/{taxAreaId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [taxArea](../resources/taxarea.md) object.

The following table shows the properties that are required when you create the [taxArea](../resources/taxarea.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|taxType|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [taxArea](../resources/taxarea.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_taxarea"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/financials/companies/{companyId}/taxAreas/{taxAreaId}
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.taxArea",
  "code": "Code value",
  "displayName": "Display Name value",
  "taxType": "Tax Type value"
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
Content-Length: 259

{
  "@odata.type": "#microsoft.graph.taxArea",
  "id": "4c848521-8521-4c84-2185-844c2185844c",
  "code": "Code value",
  "displayName": "Display Name value",
  "taxType": "Tax Type value",
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
}
```

