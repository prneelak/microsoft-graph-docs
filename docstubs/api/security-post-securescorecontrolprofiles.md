---
title: "Add secureScoreControlProfiles"
description: "Add secureScoreControlProfiles by posting to the secureScoreControlProfiles collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add secureScoreControlProfiles

Namespace: microsoft.graph

Add secureScoreControlProfiles by posting to the secureScoreControlProfiles collection.

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
POST /Security/secureScoreControlProfiles/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.

The following table shows the properties that are required when you create the [secureScoreControlProfile](../resources/securescorecontrolprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|actionType|String||
|actionUrl|String||
|azureTenantId|String||
|complianceInformation|[complianceInformation](../resources/complianceinformation.md) collection||
|controlCategory|String||
|controlStateUpdates|[secureScoreControlStateUpdate](../resources/securescorecontrolstateupdate.md) collection||
|deprecated|Boolean||
|implementationCost|String||
|lastModifiedDateTime|DateTimeOffset||
|maxScore|Double||
|rank|Int32||
|remediation|String||
|remediationImpact|String||
|service|String||
|threats|String collection||
|tier|String||
|title|String||
|userImpact|String||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||



## Response
If successful, this method returns a `201 Created` response code and a [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_securescorecontrolprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/secureScoreControlProfiles
Content-type: application/json
Content-length: 1565

{
  "@odata.type": "#microsoft.graph.secureScoreControlProfile",
  "actionType": "Action Type value",
  "actionUrl": "https://example.com/actionUrl/",
  "azureTenantId": "Azure Tenant Id value",
  "complianceInformation": [
    {
      "@odata.type": "microsoft.graph.complianceInformation",
      "certificationControls": [
        {
          "@odata.type": "microsoft.graph.certificationControl",
          "name": "Name value",
          "url": "Url value"
        }
      ],
      "certificationName": "Certification Name value"
    }
  ],
  "controlCategory": "Control Category value",
  "controlStateUpdates": [
    {
      "@odata.type": "microsoft.graph.secureScoreControlStateUpdate",
      "assignedTo": "Assigned To value",
      "comment": "Comment value",
      "state": "State value",
      "updatedBy": "Updated By value",
      "updatedDateTime": "2017-01-01T00:00:30.4198162+03:00"
    }
  ],
  "deprecated": true,
  "implementationCost": "Implementation Cost value",
  "maxScore": "Double",
  "rank": 4,
  "remediation": "Remediation value",
  "remediationImpact": "Remediation Impact value",
  "service": "Service value",
  "threats": [
    "Threats value"
  ],
  "tier": "Tier value",
  "title": "Title value",
  "userImpact": "User Impact value",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securescorecontrolprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1678

{
  "@odata.type": "#microsoft.graph.secureScoreControlProfile",
  "id": "11694b24-4b24-1169-244b-6911244b6911",
  "actionType": "Action Type value",
  "actionUrl": "https://example.com/actionUrl/",
  "azureTenantId": "Azure Tenant Id value",
  "complianceInformation": [
    {
      "@odata.type": "microsoft.graph.complianceInformation",
      "certificationControls": [
        {
          "@odata.type": "microsoft.graph.certificationControl",
          "name": "Name value",
          "url": "Url value"
        }
      ],
      "certificationName": "Certification Name value"
    }
  ],
  "controlCategory": "Control Category value",
  "controlStateUpdates": [
    {
      "@odata.type": "microsoft.graph.secureScoreControlStateUpdate",
      "assignedTo": "Assigned To value",
      "comment": "Comment value",
      "state": "State value",
      "updatedBy": "Updated By value",
      "updatedDateTime": "2017-01-01T00:00:30.4198162+03:00"
    }
  ],
  "deprecated": true,
  "implementationCost": "Implementation Cost value",
  "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
  "maxScore": "Double",
  "rank": 4,
  "remediation": "Remediation value",
  "remediationImpact": "Remediation Impact value",
  "service": "Service value",
  "threats": [
    "Threats value"
  ],
  "tier": "Tier value",
  "title": "Title value",
  "userImpact": "User Impact value",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  }
}
```

