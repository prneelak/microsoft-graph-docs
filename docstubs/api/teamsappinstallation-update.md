---
title: "Update teamsAppInstallation"
description: "Update the properties of a teamsAppInstallation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsAppInstallation

Namespace: microsoft.graph

Update the properties of a [teamsAppInstallation](../resources/teamsappinstallation.md) object.

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
PATCH /teams/{teamsId}/installedApps/{teamsAppInstallationId}
PATCH /me/joinedTeams/{groupId}/team/installedApps/{teamsAppInstallationId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [teamsAppInstallation](../resources/teamsappinstallation.md) object.

The following table shows the properties that are required when you create the [teamsAppInstallation](../resources/teamsappinstallation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsAppInstallation](../resources/teamsappinstallation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamsappinstallation"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/teams/{teamsId}/installedApps/{teamsAppInstallationId}
Content-type: application/json
Content-length: 62

{
  "@odata.type": "#microsoft.graph.teamsAppInstallation"
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
Content-Length: 111

{
  "@odata.type": "#microsoft.graph.teamsAppInstallation",
  "id": "4acba9bf-a9bf-4acb-bfa9-cb4abfa9cb4a"
}
```

