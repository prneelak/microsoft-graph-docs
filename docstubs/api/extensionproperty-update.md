---
title: "Update extensionProperty"
description: "Update the properties of a extensionProperty object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update extensionProperty

Namespace: microsoft.graph

Update the properties of a [extensionProperty](../resources/extensionproperty.md) object.

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
PATCH /applications/{applicationsId}/extensionProperties/{extensionPropertyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [extensionProperty](../resources/extensionproperty.md) object.

The following table shows the properties that are required when you create the [extensionProperty](../resources/extensionproperty.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|appDisplayName|String||
|name|String||
|dataType|String||
|isSyncedFromOnPremises|Boolean||
|targetObjects|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [extensionProperty](../resources/extensionproperty.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_extensionproperty"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/{applicationsId}/extensionProperties/{extensionPropertyId}
Content-type: application/json
Content-length: 315

{
  "@odata.type": "#microsoft.graph.extensionProperty",
  "deletedDateTime": "2016-12-31T23:59:29.9270269+00:00",
  "appDisplayName": "App Display Name value",
  "name": "Name value",
  "dataType": "Data Type value",
  "isSyncedFromOnPremises": true,
  "targetObjects": [
    "Target Objects value"
  ]
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
Content-Length: 364

{
  "@odata.type": "#microsoft.graph.extensionProperty",
  "id": "7d06609e-609e-7d06-9e60-067d9e60067d",
  "deletedDateTime": "2016-12-31T23:59:29.9270269+00:00",
  "appDisplayName": "App Display Name value",
  "name": "Name value",
  "dataType": "Data Type value",
  "isSyncedFromOnPremises": true,
  "targetObjects": [
    "Target Objects value"
  ]
}
```

