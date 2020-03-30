---
title: "Update endpoint"
description: "Update the properties of a endpoint object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update endpoint

Namespace: microsoft.graph

Update the properties of a [endpoint](../resources/endpoint.md) object.

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
PATCH /groups/{groupsId}/endpoints/{endpointId}
PATCH /me/joinedGroups/{groupId}/endpoints/{endpointId}
PATCH /servicePrincipals/{servicePrincipalsId}/endpoints/{endpointId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [endpoint](../resources/endpoint.md) object.

The following table shows the properties that are required when you create the [endpoint](../resources/endpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|capability|String||
|providerId|String||
|providerName|String||
|uri|String||
|providerResourceId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [endpoint](../resources/endpoint.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_endpoint"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}/endpoints/{endpointId}
Content-type: application/json
Content-length: 304

{
  "@odata.type": "#microsoft.graph.endpoint",
  "deletedDateTime": "2016-12-31T23:58:25.7164101+03:00",
  "capability": "Capability value",
  "providerId": "Provider Id value",
  "providerName": "Provider Name value",
  "uri": "Uri value",
  "providerResourceId": "Provider Resource Id value"
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
Content-Length: 353

{
  "@odata.type": "#microsoft.graph.endpoint",
  "id": "36f64b74-4b74-36f6-744b-f636744bf636",
  "deletedDateTime": "2016-12-31T23:58:25.7164101+03:00",
  "capability": "Capability value",
  "providerId": "Provider Id value",
  "providerName": "Provider Name value",
  "uri": "Uri value",
  "providerResourceId": "Provider Resource Id value"
}
```

