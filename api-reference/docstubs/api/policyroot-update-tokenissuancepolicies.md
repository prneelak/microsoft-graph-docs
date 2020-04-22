---
title: "Update tokenIssuancePolicies"
description: "Update the properties of a tokenIssuancePolicies object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update tokenIssuancePolicies

Namespace: microsoft.graph

Update the properties of a tokenIssuancePolicies object.

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
PATCH /policies/tokenIssuancePolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.

The following table shows the properties that are required when you create the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_tokenissuancepolicies"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/tokenIssuancePolicies
Content-Type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.tokenIssuancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
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
  "@odata.type": "#microsoft.graph.tokenIssuancePolicy",
  "id": "cc3181b2-81b2-cc31-b281-31ccb28131cc",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
}
```

