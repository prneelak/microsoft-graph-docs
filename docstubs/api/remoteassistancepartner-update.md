---
title: "Update remoteAssistancePartner"
description: "Update the properties of a remoteAssistancePartner object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update remoteAssistancePartner

Namespace: microsoft.graph

Update the properties of a [remoteAssistancePartner](../resources/remoteassistancepartner.md) object.

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
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/remoteassistancepartner.md) object.

The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/remoteassistancepartner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Display name of the partner.|
|onboardingUrl|String|URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.|
|onboardingStatus|Enumeration|TBD. Possible values are: `notOnboarded`, `onboarding`, `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Timestamp of the last request sent to Intune by the TEM partner.|



## Response
If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/remoteassistancepartner.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_remoteassistancepartner"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 262

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "2017-01-01T00:03:05.1942522+03:00"
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
Content-Length: 311

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "46626fe7-6fe7-4662-e76f-6246e76f6246",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "2017-01-01T00:03:05.1942522+03:00"
}
```

