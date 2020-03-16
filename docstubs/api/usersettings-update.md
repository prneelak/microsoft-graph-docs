---
title: "Update userSettings"
description: "Update the properties of a userSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userSettings

Namespace: microsoft.graph

Update the properties of a [userSettings](../resources/usersettings.md) object.

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
PATCH /me/settings
PATCH /users/{usersId}/settings
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userSettings](../resources/usersettings.md) object.

The following table shows the properties that are required when you create the [userSettings](../resources/usersettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|contributionToContentDiscoveryDisabled|Boolean||
|contributionToContentDiscoveryAsOrganizationDisabled|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [userSettings](../resources/usersettings.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_usersettings"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/settings
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 219

{
  "@odata.type": "#microsoft.graph.userSettings",
  "id": "569a60a8-60a8-569a-a860-9a56a8609a56",
  "contributionToContentDiscoveryDisabled": true,
  "contributionToContentDiscoveryAsOrganizationDisabled": true
}
```

