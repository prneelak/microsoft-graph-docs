---
title: "Delete directoryDefinition"
description: "Deletes a directoryDefinition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete directoryDefinition

Namespace: microsoft.graph

Deletes a [directoryDefinition](../resources/directorydefinition.md).

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
DELETE /directories/{directoriesId}
DELETE /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/directories/{directoryDefinitionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "delete_directorydefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/directories/{directoriesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

