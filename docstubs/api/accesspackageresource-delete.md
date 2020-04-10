---
title: "Delete accessPackageResource"
description: "Deletes a accessPackageResource."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete accessPackageResource

Namespace: microsoft.graph

Deletes a [accessPackageResource](../resources/accesspackageresource.md).

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
DELETE /accessPackageResources/{accessPackageResourcesId}
DELETE /identityGovernance/entitlementManagement/accessPackageResources/{accessPackageResourceId}
DELETE /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResources/{accessPackageResourceId}
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}/accessPackageResourceRoles/{accessPackageResourceRoleId}/accessPackageResource
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}/accessPackageResourceScopes/{accessPackageResourceScopeId}/accessPackageResource
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
<!-- {
  "blockType": "request",
  "name": "delete_accesspackageresource"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/accessPackageResources/{accessPackageResourcesId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

