---
title: "Add windowsInformationProtectionNetworkLearningSummaries"
description: "Add windowsInformationProtectionNetworkLearningSummaries by posting to the windowsInformationProtectionNetworkLearningSummaries collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add windowsInformationProtectionNetworkLearningSummaries

Namespace: microsoft.graph

Add windowsInformationProtectionNetworkLearningSummaries by posting to the windowsInformationProtectionNetworkLearningSummaries collection.

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
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) object.

The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|url|String|Website url|
|deviceCount|Int32|Device Count|



## Response
If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_windowsinformationprotectionnetworklearningsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
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
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsinformationprotectionnetworklearningsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "0a39b4b7-b4b7-0a39-b7b4-390ab7b4390a",
  "url": "Url value",
  "deviceCount": 11
}
```

