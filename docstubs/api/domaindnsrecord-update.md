---
title: "Update domainDnsRecord"
description: "Update the properties of a domainDnsRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update domainDnsRecord

Namespace: microsoft.graph

Update the properties of a [domainDnsRecord](../resources/domaindnsrecord.md) object.

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
PATCH /domainDnsRecords/{domainDnsRecordsId}
PATCH /domains/{domainsId}/verificationDnsRecords/{domainDnsRecordId}
PATCH /domains/{domainsId}/serviceConfigurationRecords/{domainDnsRecordId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [domainDnsRecord](../resources/domaindnsrecord.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_domaindnsrecord"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/domainDnsRecords/{domainDnsRecordsId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.domainDnsRecord",
  "id": "c81982f5-82f5-c819-f582-19c8f58219c8",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3
}
```

