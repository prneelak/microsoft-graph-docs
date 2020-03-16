---
title: "Update teamsApp"
description: "Update the properties of a teamsApp object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsApp

Namespace: microsoft.graph

Update the properties of a [teamsApp](../resources/teamsapp.md) object.

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
PATCH /appCatalogs/teamsApps/{teamsAppId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [teamsApp](../resources/teamsapp.md) object.

The following table shows the properties that are required when you create the [teamsApp](../resources/teamsapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|externalId|String||
|displayName|String||
|distributionMethod|Enumeration|. Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsApp](../resources/teamsapp.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/appCatalogs/teamsApps/{teamsAppId}
Content-type: application/json
Content-length: 163

{
  "@odata.type": "#microsoft.graph.teamsApp",
  "externalId": "External Id value",
  "displayName": "Display Name value",
  "distributionMethod": "String"
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
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.teamsApp",
  "id": "c7c9c3f2-c3f2-c7c9-f2c3-c9c7f2c3c9c7",
  "externalId": "External Id value",
  "displayName": "Display Name value",
  "distributionMethod": "String"
}
```

