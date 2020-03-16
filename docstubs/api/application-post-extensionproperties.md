---
title: "Add extensionProperties"
description: "Add extensionProperties by posting to the extensionProperties collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add extensionProperties

Namespace: microsoft.graph

Add extensionProperties by posting to the extensionProperties collection.

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
POST /applications/{applicationsId}/extensionProperties/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [extensionProperty](../resources/extensionproperty.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_extensionproperty_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/applications/{applicationsId}/extensionProperties
Content-type: application/json
Content-length: 315

{
  "@odata.type": "#microsoft.graph.extensionProperty",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionproperty"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 364

{
  "@odata.type": "#microsoft.graph.extensionProperty",
  "id": "8c26eb49-eb49-8c26-49eb-268c49eb268c",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "appDisplayName": "App Display Name value",
  "name": "Name value",
  "dataType": "Data Type value",
  "isSyncedFromOnPremises": true,
  "targetObjects": [
    "Target Objects value"
  ]
}
```

