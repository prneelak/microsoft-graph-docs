---
title: "Add appliedPolicies"
description: "Add appliedPolicies by posting to the appliedPolicies collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add appliedPolicies

Namespace: microsoft.graph

Add appliedPolicies by posting to the appliedPolicies collection.

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
POST /me/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedAppPolicy](../resources/managedapppolicy.md) object.

The following table shows the properties that are required when you create the [managedAppPolicy](../resources/managedapppolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Policy display name.|
|description|String|The policy's description.|
|createdDateTime|DateTimeOffset|The date and time the policy was created.|
|lastModifiedDateTime|DateTimeOffset|Last time the policy was modified.|
|version|String|Version of the entity.|



## Response
If successful, this method returns a `201 Created` response code and a [managedAppPolicy](../resources/managedapppolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managedapppolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedapppolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 340

{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "id": "0037cbf9-cbf9-0037-f9cb-3700f9cb3700",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:00:51.2796212+03:00",
  "lastModifiedDateTime": "2016-12-31T23:57:58.0056135+03:00",
  "version": "Version value"
}
```

