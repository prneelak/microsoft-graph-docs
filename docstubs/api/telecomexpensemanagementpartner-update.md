---
title: "Update telecomExpenseManagementPartner"
description: "Update the properties of a telecomExpenseManagementPartner object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update telecomExpenseManagementPartner

Namespace: microsoft.graph

Update the properties of a [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object.

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
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object.

The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Display name of the TEM partner.|
|url|String|URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.|
|appAuthorized|Boolean|Whether the partner's AAD app has been authorized to access Intune.|
|enabled|Boolean|Whether Intune's connection to the TEM service is currently enabled or disabled.|
|lastConnectionDateTime|DateTimeOffset|Timestamp of the last request sent to Intune by the TEM partner.|



## Response
If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_telecomexpensemanagementpartner"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
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
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "7b5c1645-1645-7b5c-4516-5c7b45165c7b",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2017-01-01T00:03:05.1942522+03:00"
}
```

