---
title: "List appliedPolicies"
description: "Get the managedAppPolicies from the appliedPolicies navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List appliedPolicies

Namespace: microsoft.graph

Get the managedAppPolicies from the appliedPolicies navigation property.

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
GET /me/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [managedAppPolicy](../resources/managedapppolicy.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_managedapppolicy"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.managedapppolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "id": "885196a0-96a0-8851-a096-5188a0965188",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
      "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
      "version": "Version value"
    }
  ]
}
```

