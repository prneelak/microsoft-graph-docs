---
title: "Update providerTenantSetting"
description: "Update the properties of a providerTenantSetting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update providerTenantSetting

Namespace: microsoft.graph

Update the properties of a [providerTenantSetting](../resources/providertenantsetting.md) object.

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
PATCH /Security/providerTenantSettings/{providerTenantSettingId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [providerTenantSetting](../resources/providertenantsetting.md) object.

The following table shows the properties that are required when you create the [providerTenantSetting](../resources/providertenantsetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|azureTenantId|String||
|enabled|Boolean||
|lastModifiedDateTime|DateTimeOffset||
|provider|String||
|vendor|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [providerTenantSetting](../resources/providertenantsetting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_providertenantsetting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/providerTenantSettings/{providerTenantSettingId}
Content-type: application/json
Content-length: 190

{
  "@odata.type": "#microsoft.graph.providerTenantSetting",
  "azureTenantId": "Azure Tenant Id value",
  "enabled": true,
  "provider": "Provider value",
  "vendor": "Vendor value"
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
Content-Length: 303

{
  "@odata.type": "#microsoft.graph.providerTenantSetting",
  "id": "31bbb11d-b11d-31bb-1db1-bb311db1bb31",
  "azureTenantId": "Azure Tenant Id value",
  "enabled": true,
  "lastModifiedDateTime": "2017-01-01T00:02:50.3839766+00:00",
  "provider": "Provider value",
  "vendor": "Vendor value"
}
```

