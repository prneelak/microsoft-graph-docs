---
title: "Add protectedAppLockerFiles"
description: "Add protectedAppLockerFiles by posting to the protectedAppLockerFiles collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add protectedAppLockerFiles

Namespace: microsoft.graph

Add protectedAppLockerFiles by posting to the protectedAppLockerFiles collection.

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
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object.

The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The friendly name|
|fileHash|String|SHA256 hash of the file|
|file|Binary|File as a byte array|
|version|String|Version of the entity.|



## Response
If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_windowsinformationprotectionapplockerfile_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsinformationprotectionapplockerfile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "id": "14554736-4736-1455-3647-551436475514",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

