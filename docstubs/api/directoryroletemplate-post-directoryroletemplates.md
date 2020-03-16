---
title: "Create directoryRoleTemplate"
description: "Create a new directoryRoleTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create directoryRoleTemplate

Namespace: microsoft.graph

Create a new [directoryRoleTemplate](../resources/directoryroletemplate.md) object.

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
POST /directoryRoleTemplates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [directoryRoleTemplate](../resources/directoryroletemplate.md) object.

The following table shows the properties that are required when you create the [directoryRoleTemplate](../resources/directoryroletemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String||
|displayName|String||



## Response
If successful, this method returns a `201 Created` response code and a [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_directoryroletemplate_from_directoryroletemplates"
}
-->
``` http
POST https://graph.microsoft.com/localtest/directoryRoleTemplates
Content-type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.directoryRoleTemplate",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "description": "Description value",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryroletemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 250

{
  "@odata.type": "#microsoft.graph.directoryRoleTemplate",
  "id": "834a4c59-4c59-834a-594c-4a83594c4a83",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "description": "Description value",
  "displayName": "Display Name value"
}
```

