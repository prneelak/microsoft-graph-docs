---
title: "Update sectionGroup"
description: "Update the properties of a sectionGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update sectionGroup

Namespace: microsoft.graph

Update the properties of a [sectionGroup](../resources/sectiongroup.md) object.

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
PATCH /me/onenote/sectionGroups/{sectionGroupId}
PATCH /me/onenote/notebooks/{notebookId}/sectionGroups/{sectionGroupId}
PATCH /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup
PATCH /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/parentSectionGroup
PATCH /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/sectionGroups/{sectionGroupId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [sectionGroup](../resources/sectiongroup.md) object.

The following table shows the properties that are required when you create the [sectionGroup](../resources/sectiongroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|displayName|String| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|sectionsUrl|String||
|sectionGroupsUrl|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [sectionGroup](../resources/sectiongroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_sectiongroup"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/onenote/sectionGroups/{sectionGroupId}
Content-type: application/json
Content-length: 561

{
  "@odata.type": "#microsoft.graph.sectionGroup",
  "self": "Self value",
  "displayName": "Display Name value",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "sectionsUrl": "https://example.com/sectionsUrl/",
  "sectionGroupsUrl": "https://example.com/sectionGroupsUrl/"
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
Content-Length: 812

{
  "@odata.type": "#microsoft.graph.sectionGroup",
  "id": "9c856a38-6a38-9c85-386a-859c386a859c",
  "self": "Self value",
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "displayName": "Display Name value",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "sectionsUrl": "https://example.com/sectionsUrl/",
  "sectionGroupsUrl": "https://example.com/sectionGroupsUrl/"
}
```

