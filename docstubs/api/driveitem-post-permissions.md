---
title: "Add permissions"
description: "Add permissions by posting to the permissions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add permissions

Namespace: microsoft.graph

Add permissions by posting to the permissions collection.

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
POST /workbooks/{workbooksId}/permissions/$ref
POST /me/drive/items/{driveItemId}/permissions/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [permission](../resources/permission.md) object.

The following table shows the properties that are required when you create the [permission](../resources/permission.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|grantedTo|[identitySet](../resources/identityset.md)||
|inheritedFrom|[itemReference](../resources/itemreference.md)||
|invitation|[sharingInvitation](../resources/sharinginvitation.md)||
|link|[sharingLink](../resources/sharinglink.md)||
|roles|String collection||
|shareId|String||



## Response
If successful, this method returns a `201 Created` response code and a [permission](../resources/permission.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_permission_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/workbooks/{workbooksId}/permissions
Content-type: application/json
Content-length: 1496

{
  "@odata.type": "#microsoft.graph.permission",
  "grantedTo": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "inheritedFrom": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "Drive Id value",
    "driveType": "Drive Type value",
    "name": "Name value",
    "path": "Path value",
    "shareId": "Share Id value",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "List Id value",
      "listItemId": "List Item Id value",
      "listItemUniqueId": "List Item Unique Id value",
      "siteId": "Site Id value",
      "siteUrl": "https://example.com/siteUrl/",
      "webId": "Web Id value"
    }
  },
  "invitation": {
    "@odata.type": "microsoft.graph.sharingInvitation",
    "email": "Email value",
    "invitedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "redeemedBy": "Redeemed By value",
    "signInRequired": true
  },
  "link": {
    "@odata.type": "microsoft.graph.sharingLink",
    "scope": "Scope value",
    "type": "Type value",
    "webUrl": "https://example.com/webUrl/"
  },
  "roles": [
    "Roles value"
  ],
  "shareId": "Share Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1545

{
  "@odata.type": "#microsoft.graph.permission",
  "id": "138e3be6-3be6-138e-e63b-8e13e63b8e13",
  "grantedTo": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "inheritedFrom": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "Drive Id value",
    "driveType": "Drive Type value",
    "name": "Name value",
    "path": "Path value",
    "shareId": "Share Id value",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "List Id value",
      "listItemId": "List Item Id value",
      "listItemUniqueId": "List Item Unique Id value",
      "siteId": "Site Id value",
      "siteUrl": "https://example.com/siteUrl/",
      "webId": "Web Id value"
    }
  },
  "invitation": {
    "@odata.type": "microsoft.graph.sharingInvitation",
    "email": "Email value",
    "invitedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "redeemedBy": "Redeemed By value",
    "signInRequired": true
  },
  "link": {
    "@odata.type": "microsoft.graph.sharingLink",
    "scope": "Scope value",
    "type": "Type value",
    "webUrl": "https://example.com/webUrl/"
  },
  "roles": [
    "Roles value"
  ],
  "shareId": "Share Id value"
}
```

