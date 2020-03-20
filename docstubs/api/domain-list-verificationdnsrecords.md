---
title: "List verificationDnsRecords"
description: "Get the domainDnsRecords from the verificationDnsRecords navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List verificationDnsRecords

Namespace: microsoft.graph

Get the domainDnsRecords from the verificationDnsRecords navigation property.

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
GET /domains/{domainsId}/verificationDnsRecords
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
If successful, this method returns a `200 OK` response code and a collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domaindnsrecord"
}
-->
``` http
GET https://graph.microsoft.com/localtest/domains/{domainsId}/verificationDnsRecords
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.domaindnsrecord)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.domainDnsRecord",
      "id": "cc00a1f4-a1f4-cc00-f4a1-00ccf4a100cc",
      "isOptional": true,
      "label": "Label value",
      "recordType": "Record Type value",
      "supportedService": "Supported Service value",
      "ttl": 3
    }
  ]
}
```

