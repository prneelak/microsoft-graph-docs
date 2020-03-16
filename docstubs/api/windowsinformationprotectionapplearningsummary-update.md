---
title: "Update windowsInformationProtectionAppLearningSummary"
description: "Update the properties of a windowsInformationProtectionAppLearningSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update windowsInformationProtectionAppLearningSummary

Namespace: microsoft.graph

Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object.

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
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object.

The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|applicationName|String|Application Name|
|applicationType|Enumeration|Application Type. Possible values are: `universal`, `desktop`.|
|deviceCount|Int32|Device Count|



## Response
If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_windowsinformationprotectionapplearningsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 190

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "String",
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
Content-Length: 239

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "ab0f5cf0-5cf0-ab0f-f05c-0fabf05c0fab",
  "applicationName": "Application Name value",
  "applicationType": "String",
  "deviceCount": 11
}
```

