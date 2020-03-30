---
title: "Add teamsApps"
description: "Add teamsApps by posting to the teamsApps collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add teamsApps

Namespace: microsoft.graph

Add teamsApps by posting to the teamsApps collection.

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
POST /appCatalogs/teamsApps/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [teamsApp](../resources/teamsapp.md) object.

The following table shows the properties that are required when you create the [teamsApp](../resources/teamsapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|externalId|String||
|name|String||
|displayName|String||
|distributionMethod|Enumeration| Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [teamsApp](../resources/teamsapp.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_teamsapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/json
Content-length: 188

{
  "@odata.type": "#microsoft.graph.teamsApp",
  "externalId": "External Id value",
  "name": "Name value",
  "displayName": "Display Name value",
  "distributionMethod": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsapp"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 237

{
  "@odata.type": "#microsoft.graph.teamsApp",
  "id": "a36ea462-a462-a36e-62a4-6ea362a46ea3",
  "externalId": "External Id value",
  "name": "Name value",
  "displayName": "Display Name value",
  "distributionMethod": "String"
}
```

