---
title: "Update entitlementManagement"
description: "Update the properties of an entitlementManagement object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update entitlementManagement

Namespace: microsoft.graph

Update the properties of an [entitlementManagement](../resources/entitlementmanagement.md) object.

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
PATCH /entitlementManagement
PATCH /identityGovernance/entitlementManagement
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [entitlementManagement](../resources/entitlementmanagement.md) object.

The following table shows the properties that are required when you create the [entitlementManagement](../resources/entitlementmanagement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response

If successful, this method returns a `200 OK` response code and an updated [entitlementManagement](../resources/entitlementmanagement.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_entitlementmanagement"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/entitlementManagement
Content-Type: application/json
Content-length: 63

{
  "@odata.type": "#microsoft.graph.entitlementManagement"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.entitlementManagement",
  "id": "d45ea2b8-a2b8-d45e-b8a2-5ed4b8a25ed4"
}
```

