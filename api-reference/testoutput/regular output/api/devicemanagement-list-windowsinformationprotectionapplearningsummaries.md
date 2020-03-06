---
title: "List windowsInformationProtectionAppLearningSummaries"
description: "Get the windowsInformationProtectionAppLearningSummaries from the windowsInformationProtectionAppLearningSummaries navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List windowsInformationProtectionAppLearningSummaries

Namespace: microsoft.graph

Get the windowsInformationProtectionAppLearningSummaries from the windowsInformationProtectionAppLearningSummaries navigation property.

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
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsinformationprotectionapplearningsummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/windowsInformationProtectionAppLearningSummaries
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsinformationprotectionapplearningsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 292

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
      "id": "b5551e0d-1e0d-b555-0d1e-55b50d1e55b5",
      "applicationName": "Application Name value",
      "applicationType": "String",
      "deviceCount": 11
    }
  ]
}
```

