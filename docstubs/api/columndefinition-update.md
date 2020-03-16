---
title: "Update columnDefinition"
description: "Update the properties of a columnDefinition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update columnDefinition

Namespace: microsoft.graph

Update the properties of a [columnDefinition](../resources/columndefinition.md) object.

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
PATCH /me/drive/list/columns/{columnDefinitionId}
PATCH /sites/{sitesId}/columns/{columnDefinitionId}
PATCH /me/joinedTeams/{groupId}/sites/{siteId}/columns/{columnDefinitionId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [columnDefinition](../resources/columndefinition.md) object.

The following table shows the properties that are required when you create the [columnDefinition](../resources/columndefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|boolean|[booleanColumn](../resources/booleancolumn.md)||
|calculated|[calculatedColumn](../resources/calculatedcolumn.md)||
|choice|[choiceColumn](../resources/choicecolumn.md)||
|columnGroup|String||
|currency|[currencyColumn](../resources/currencycolumn.md)||
|dateTime|[dateTimeColumn](../resources/datetimecolumn.md)||
|defaultValue|[defaultColumnValue](../resources/defaultcolumnvalue.md)||
|description|String||
|displayName|String||
|enforceUniqueValues|Boolean||
|hidden|Boolean||
|indexed|Boolean||
|lookup|[lookupColumn](../resources/lookupcolumn.md)||
|name|String||
|number|[numberColumn](../resources/numbercolumn.md)||
|personOrGroup|[personOrGroupColumn](../resources/personorgroupcolumn.md)||
|readOnly|Boolean||
|required|Boolean||
|text|[textColumn](../resources/textcolumn.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [columnDefinition](../resources/columndefinition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_columndefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/list/columns/{columnDefinitionId}
Content-type: application/json
Content-length: 1904

{
  "@odata.type": "#microsoft.graph.columnDefinition",
  "boolean": {
    "@odata.type": "microsoft.graph.booleanColumn"
  },
  "calculated": {
    "@odata.type": "microsoft.graph.calculatedColumn",
    "format": "Format value",
    "formula": "Formula value",
    "outputType": "Output Type value"
  },
  "choice": {
    "@odata.type": "microsoft.graph.choiceColumn",
    "allowTextEntry": true,
    "choices": [
      "Choices value"
    ],
    "displayAs": "Display As value"
  },
  "columnGroup": "Column Group value",
  "currency": {
    "@odata.type": "microsoft.graph.currencyColumn",
    "locale": "Locale value"
  },
  "dateTime": {
    "@odata.type": "microsoft.graph.dateTimeColumn"
  },
  "defaultValue": {
    "@odata.type": "microsoft.graph.defaultColumnValue",
    "value": "Value value"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "enforceUniqueValues": true,
  "hidden": true,
  "indexed": true,
  "lookup": {
    "@odata.type": "microsoft.graph.lookupColumn",
    "allowMultipleValues": true,
    "allowUnlimitedLength": true,
    "columnName": "Column Name value",
    "listId": "List Id value",
    "primaryLookupColumnId": "Primary Lookup Column Id value"
  },
  "name": "Name value",
  "number": {
    "@odata.type": "microsoft.graph.numberColumn",
    "decimalPlaces": "Decimal Places value",
    "maximum": "Double",
    "minimum": "Double"
  },
  "personOrGroup": {
    "@odata.type": "microsoft.graph.personOrGroupColumn",
    "allowMultipleSelection": true,
    "chooseFromType": "Choose From Type value"
  },
  "readOnly": true,
  "required": true,
  "text": {
    "@odata.type": "microsoft.graph.textColumn",
    "allowMultipleLines": true,
    "appendChangesToExistingText": true,
    "linesForEditing": 15,
    "maxLength": 9,
    "textType": "Text Type value"
  }
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
Content-Length: 1953

{
  "@odata.type": "#microsoft.graph.columnDefinition",
  "id": "fcae4f9b-4f9b-fcae-9b4f-aefc9b4faefc",
  "boolean": {
    "@odata.type": "microsoft.graph.booleanColumn"
  },
  "calculated": {
    "@odata.type": "microsoft.graph.calculatedColumn",
    "format": "Format value",
    "formula": "Formula value",
    "outputType": "Output Type value"
  },
  "choice": {
    "@odata.type": "microsoft.graph.choiceColumn",
    "allowTextEntry": true,
    "choices": [
      "Choices value"
    ],
    "displayAs": "Display As value"
  },
  "columnGroup": "Column Group value",
  "currency": {
    "@odata.type": "microsoft.graph.currencyColumn",
    "locale": "Locale value"
  },
  "dateTime": {
    "@odata.type": "microsoft.graph.dateTimeColumn"
  },
  "defaultValue": {
    "@odata.type": "microsoft.graph.defaultColumnValue",
    "value": "Value value"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "enforceUniqueValues": true,
  "hidden": true,
  "indexed": true,
  "lookup": {
    "@odata.type": "microsoft.graph.lookupColumn",
    "allowMultipleValues": true,
    "allowUnlimitedLength": true,
    "columnName": "Column Name value",
    "listId": "List Id value",
    "primaryLookupColumnId": "Primary Lookup Column Id value"
  },
  "name": "Name value",
  "number": {
    "@odata.type": "microsoft.graph.numberColumn",
    "decimalPlaces": "Decimal Places value",
    "maximum": "Double",
    "minimum": "Double"
  },
  "personOrGroup": {
    "@odata.type": "microsoft.graph.personOrGroupColumn",
    "allowMultipleSelection": true,
    "chooseFromType": "Choose From Type value"
  },
  "readOnly": true,
  "required": true,
  "text": {
    "@odata.type": "microsoft.graph.textColumn",
    "allowMultipleLines": true,
    "appendChangesToExistingText": true,
    "linesForEditing": 15,
    "maxLength": 9,
    "textType": "Text Type value"
  }
}
```

