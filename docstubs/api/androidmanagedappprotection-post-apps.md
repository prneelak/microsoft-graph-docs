---
title: "Add apps"
description: "Add apps by posting to the apps collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add apps

Namespace: microsoft.graph

Add apps by posting to the apps collection.

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
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedMobileApp](../resources/managedmobileapp.md) object.

The following table shows the properties that are required when you create the [managedMobileApp](../resources/managedmobileapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)|The identifier for an app with it's operating system type.|
|version|String|Version of the entity.|



## Response
If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/managedmobileapp.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managedmobileapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedmobileapp"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "id": "0115ddc6-ddc6-0115-c6dd-1501c6dd1501",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

