---
title: "Create managementConditionStatements"
description: "Create managementConditionStatements by posting to the managementConditionStatements collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create managementConditionStatements

Namespace: microsoft.graph

Create managementConditionStatements by posting to the managementConditionStatements collection.

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
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managementConditionStatement](../resources/managementconditionstatement.md) object.

The following table shows the properties that are required when you create the [managementConditionStatement](../resources/managementconditionstatement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The admin defined name of the management condition statement.|
|description|String|The admin defined description of the management condition statement.|
|createdDateTime|DateTimeOffset|The time the management condition statement was created. Generated service side.|
|modifiedDateTime|DateTimeOffset|The time the management condition statement was last modified. Updated service side.|
|expression|[managementConditionExpression](../resources/managementconditionexpression.md)|The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.|
|eTag|String|ETag of the management condition statement. Updated service side.|
|applicablePlatforms|Enumeration collection|The applicable platforms for this management condition statement.
This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|



## Response
If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/managementconditionstatement.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managementconditionstatement_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
Content-type: application/json
Content-length: 315

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "String"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managementconditionstatement"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "c008f38b-f38b-c008-8bf3-08c08bf308c0",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "modifiedDateTime": "2016-12-31T23:58:13.3996216+03:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "String"
  ]
}
```

