---
title: "Create directoryRole"
description: "Create a new directoryRole object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create directoryRole

Namespace: microsoft.graph

Create a new [directoryRole](../resources/directoryrole.md) object.

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
POST /directoryRoles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [directoryRole](../resources/directoryrole.md) object.

The following table shows the properties that are required when you create the [directoryRole](../resources/directoryrole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String||
|displayName|String||
|roleTemplateId|String||



## Response
If successful, this method returns a `201 Created` response code and a [directoryRole](../resources/directoryrole.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}
-->
``` http
POST https://graph.microsoft.com/localtest/directoryRoles
Content-type: application/json
Content-length: 240

{
  "@odata.type": "#microsoft.graph.directoryRole",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "roleTemplateId": "Role Template Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryrole"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 289

{
  "@odata.type": "#microsoft.graph.directoryRole",
  "id": "6da244ee-44ee-6da2-ee44-a26dee44a26d",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "roleTemplateId": "Role Template Id value"
}
```

