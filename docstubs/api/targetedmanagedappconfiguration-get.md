---
title: "Get targetedManagedAppConfiguration"
description: "Read properties and relationships of the targetedManagedAppConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get targetedManagedAppConfiguration

Namespace: microsoft.graph

Read properties and relationships of the [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object.

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
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_targetedmanagedappconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 679

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "id": "34721b46-1b46-3472-461b-7234461b7234",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
    "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "deployedAppCount": 0,
    "isAssigned": true
  }
}
```

