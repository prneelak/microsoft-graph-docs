---
title: "Create userSettings"
description: "Create a new userSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create userSettings

Namespace: microsoft.graph

Create a new [userSettings](../resources/usersettings.md) object.

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
POST ** Collection URI for microsoft.graph.userSettings not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [userSettings](../resources/usersettings.md) object.

The following table shows the properties that are required when you create the [userSettings](../resources/usersettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|contributionToContentDiscoveryDisabled|Boolean||
|contributionToContentDiscoveryAsOrganizationDisabled|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [userSettings](../resources/usersettings.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_usersettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.userSettings not found
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.userSettings",
  "contributionToContentDiscoveryDisabled": true,
  "contributionToContentDiscoveryAsOrganizationDisabled": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usersettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 219

{
  "@odata.type": "#microsoft.graph.userSettings",
  "id": "dd01d35c-d35c-dd01-5cd3-01dd5cd301dd",
  "contributionToContentDiscoveryDisabled": true,
  "contributionToContentDiscoveryAsOrganizationDisabled": true
}
```

