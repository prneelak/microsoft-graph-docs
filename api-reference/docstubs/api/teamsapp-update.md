---
title: "Update teamsApp"
description: "Update the properties of a teamsApp object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update teamsApp

Namespace: microsoft.graph

Update the properties of a [teamsApp](../resources/teamsapp.md) object.

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
PATCH /appCatalogs/teamsApps/{teamsAppId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [teamsApp](../resources/teamsapp.md) object.

The following table shows the properties that are required when you create the [teamsApp](../resources/teamsapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|externalId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|distributionMethod|teamsAppDistributionMethod|**TODO: Add Description**. Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsApp](../resources/teamsapp.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}
Content-Type: application/json
Content-length: 163

{
  "@odata.type": "#microsoft.graph.teamsApp",
  "externalId": "External Id value",
  "displayName": "Display Name value",
  "distributionMethod": "String"
}
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
{
  "@odata.type": "#microsoft.graph.teamsApp",
  "id": "285ee313-e313-285e-13e3-5e2813e35e28",
  "externalId": "External Id value",
  "displayName": "Display Name value",
  "distributionMethod": "String"
}
```

