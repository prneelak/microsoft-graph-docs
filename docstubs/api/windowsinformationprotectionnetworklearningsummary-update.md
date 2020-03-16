---
title: "Update windowsInformationProtectionNetworkLearningSummary"
description: "Update the properties of a windowsInformationProtectionNetworkLearningSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update windowsInformationProtectionNetworkLearningSummary

Namespace: microsoft.graph

Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) object.

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
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) object.

The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|url|String|Website url|
|deviceCount|Int32|Device Count|



## Response
If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_windowsinformationprotectionnetworklearningsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
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
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "0a39b4b7-b4b7-0a39-b7b4-390ab7b4390a",
  "url": "Url value",
  "deviceCount": 11
}
```

