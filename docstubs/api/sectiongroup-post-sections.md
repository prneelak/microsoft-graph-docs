---
title: "Add sections"
description: "Add sections by posting to the sections collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add sections

Namespace: microsoft.graph

Add sections by posting to the sections collection.

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
POST /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/sections/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [onenoteSection](../resources/onenotesection.md) object.

The following table shows the properties that are required when you create the [onenoteSection](../resources/onenotesection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|displayName|String| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|isDefault|Boolean||
|links|[sectionLinks](../resources/sectionlinks.md)||
|pagesUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/onenotesection.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onenotesection_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/sections
Content-type: application/json
Content-length: 788

{
  "@odata.type": "#microsoft.graph.onenoteSection",
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
  "isDefault": true,
  "links": {
    "@odata.type": "microsoft.graph.sectionLinks",
    "oneNoteClientUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "Href value"
    },
    "oneNoteWebUrl": {
      "@odata.type": "microsoft.graph.externalLink"
    }
  },
  "pagesUrl": "https://example.com/pagesUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotesection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1039

{
  "@odata.type": "#microsoft.graph.onenoteSection",
  "id": "13b63f6a-3f6a-13b6-6a3f-b6136a3fb613",
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
  "isDefault": true,
  "links": {
    "@odata.type": "microsoft.graph.sectionLinks",
    "oneNoteClientUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "Href value"
    },
    "oneNoteWebUrl": {
      "@odata.type": "microsoft.graph.externalLink"
    }
  },
  "pagesUrl": "https://example.com/pagesUrl/"
}
```

