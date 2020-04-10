---
title: "Update teamsAppDefinition"
description: "Update the properties of a teamsAppDefinition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsAppDefinition

Namespace: microsoft.graph

Update the properties of a [teamsAppDefinition](../resources/teamsappdefinition.md) object.

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
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [teamsAppDefinition](../resources/teamsappdefinition.md) object.

The following table shows the properties that are required when you create the [teamsAppDefinition](../resources/teamsappdefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|teamsAppId|String||
|displayName|String||
|version|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsAppDefinition](../resources/teamsappdefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_teamsappdefinition"
}
-->
``` http

```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 219

{
  "@odata.type": "#microsoft.graph.teamsAppDefinition",
  "id": "9a4e8f73-8f73-9a4e-738f-4e9a738f4e9a",
  "teamsAppId": "Teams App Id value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

