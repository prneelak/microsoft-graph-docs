---
title: "Get identityUserFlow"
description: "Read the properties and relationships of an identityUserFlow object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get identityUserFlow

Namespace: microsoft.graph

Read the properties and relationships of an [identityUserFlow](../resources/identityuserflow.md) object.

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
GET /identity/userFlows/{identityUserFlowId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [identityUserFlow](../resources/identityuserflow.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_identityuserflow"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/userFlows/{identityUserFlowId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlow"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.identityUserFlow",
    "id": "4dba9023-9023-4dba-2390-ba4d2390ba4d",
    "userFlowType": "String",
    "userFlowTypeVersion": "Single"
  }
}
```

