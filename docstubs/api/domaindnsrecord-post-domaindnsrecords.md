---
title: "Create domainDnsRecord"
description: "Create a new domainDnsRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create domainDnsRecord

Namespace: microsoft.graph

Create a new [domainDnsRecord](../resources/domaindnsrecord.md) object.

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
POST /domainDnsRecords
POST /domains/{domainsId}/verificationDnsRecords
POST /domains/{domainsId}/serviceConfigurationRecords
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [domainDnsRecord](../resources/domaindnsrecord.md) object.

The following table shows the properties that are required when you create the [domainDnsRecord](../resources/domaindnsrecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean||
|label|String||
|recordType|String||
|supportedService|String||
|ttl|Int32||



## Response
If successful, this method returns a `201 Created` response code and a [domainDnsRecord](../resources/domaindnsrecord.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_domaindnsrecord_from_domaindnsrecords"
}
-->
``` http
POST https://graph.microsoft.com/localtest/domainDnsRecords
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.domainDnsRecord",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domaindnsrecord"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.domainDnsRecord",
  "id": "c9b584fe-84fe-c9b5-fe84-b5c9fe84b5c9",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3
}
```

