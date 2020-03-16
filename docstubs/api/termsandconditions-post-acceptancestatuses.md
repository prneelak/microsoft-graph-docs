---
title: "Add acceptanceStatuses"
description: "Add acceptanceStatuses by posting to the acceptanceStatuses collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add acceptanceStatuses

Namespace: microsoft.graph

Add acceptanceStatuses by posting to the acceptanceStatuses collection.

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
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object.

The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userDisplayName|String|Display name of the user whose acceptance the entity represents.|
|acceptedVersion|Int32|Most recent version number of the T&C accepted by the user.|
|acceptedDateTime|DateTimeOffset|DateTime when the terms were last accepted by the user.|



## Response
If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_termsandconditionsacceptancestatus_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2017-01-01T00:01:08.9033237+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termsandconditionsacceptancestatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "d29c9f55-9f55-d29c-559f-9cd2559f9cd2",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2017-01-01T00:01:08.9033237+03:00"
}
```

