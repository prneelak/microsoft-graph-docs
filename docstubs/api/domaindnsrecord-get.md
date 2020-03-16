---
title: "Get domainDnsRecord"
description: "Read properties and relationships of the domainDnsRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get domainDnsRecord

Namespace: microsoft.graph

Read properties and relationships of the [domainDnsRecord](../resources/domaindnsrecord.md) object.

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
GET /domainDnsRecords/{domainDnsRecordsId}
GET /domains/{domainsId}/verificationDnsRecords/{domainDnsRecordId}
GET /domains/{domainsId}/serviceConfigurationRecords/{domainDnsRecordId}
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
If successful, this method returns a `200 OK` response code and [domainDnsRecord](../resources/domaindnsrecord.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domaindnsrecord"
}
-->
``` http
GET https://graph.microsoft.com/localtest/domainDnsRecords/{domainDnsRecordsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "value": {
    "@odata.type": "#microsoft.graph.domainDnsRecord",
    "id": "c81982f5-82f5-c819-f582-19c8f58219c8",
    "isOptional": true,
    "label": "Label value",
    "recordType": "Record Type value",
    "supportedService": "Supported Service value",
    "ttl": 3
  }
}
```

