---
title: "Add mobileAppIntentAndStates"
description: "Add mobileAppIntentAndStates by posting to the mobileAppIntentAndStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add mobileAppIntentAndStates

Namespace: microsoft.graph

Add mobileAppIntentAndStates by posting to the mobileAppIntentAndStates collection.

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
POST /me/mobileAppIntentAndStates/$ref
POST /users/{usersId}/mobileAppIntentAndStates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object.

The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/mobileappintentandstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|managedDeviceIdentifier|String||
|userId|String||
|mobileAppList|[mobileAppIntentAndStateDetail](../resources/mobileappintentandstatedetail.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mobileappintentandstate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/mobileAppIntentAndStates
Content-type: application/json
Content-length: 822

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "String",
      "displayVersion": "Display Version value",
      "installState": "String",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "String",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileappintentandstate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 871

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "1500c633-c633-1500-33c6-001533c60015",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "String",
      "displayVersion": "Display Version value",
      "installState": "String",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "String",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```

