---
title: "Create directoryObjectPartnerReference"
description: "Create a new directoryObjectPartnerReference object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create directoryObjectPartnerReference

Namespace: microsoft.graph

Create a new [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object.

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
POST ** Collection URI for microsoft.graph.directoryObjectPartnerReference not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object.

The following table shows the properties that are required when you create the [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String||
|displayName|String||
|externalPartnerTenantId|Guid||
|objectType|String||



## Response
If successful, this method returns a `201 Created` response code and a [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_directoryobjectpartnerreference_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.directoryObjectPartnerReference not found
Content-type: application/json
Content-length: 319

{
  "@odata.type": "#microsoft.graph.directoryObjectPartnerReference",
  "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "externalPartnerTenantId": "189e00e4-00e4-189e-e400-9e18e4009e18",
  "objectType": "Object Type value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryobjectpartnerreference"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 368

{
  "@odata.type": "#microsoft.graph.directoryObjectPartnerReference",
  "id": "42c43b87-3b87-42c4-873b-c442873bc442",
  "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "externalPartnerTenantId": "189e00e4-00e4-189e-e400-9e18e4009e18",
  "objectType": "Object Type value"
}
```

