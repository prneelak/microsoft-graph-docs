---
title: "Update organization"
description: "Update the properties of a organization object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update organization

Namespace: microsoft.graph

Update the properties of a [organization](../resources/organization.md) object.

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
PATCH /organization/{organizationId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [organization](../resources/organization.md) object.

The following table shows the properties that are required when you create the [organization](../resources/organization.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection||
|businessPhones|String collection||
|city|String||
|country|String||
|countryLetterCode|String||
|createdDateTime|DateTimeOffset||
|creationType|String||
|displayName|String||
|marketingNotificationEmails|String collection||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesSyncEnabled|Boolean||
|postalCode|String||
|preferredLanguage|String||
|privacyProfile|[privacyProfile](../resources/privacyprofile.md)||
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection||
|securityComplianceNotificationMails|String collection||
|securityComplianceNotificationPhones|String collection||
|state|String||
|street|String||
|technicalNotificationMails|String collection||
|verifiedDomains|[verifiedDomain](../resources/verifieddomain.md) collection||
|mobileDeviceManagementAuthority|Enumeration|Mobile device management authority. Possible values are: `unknown`, `intune`, `sccm`, `office365`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [organization](../resources/organization.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_organization"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/organization/{organizationId}
Content-type: application/json
Content-length: 1943

{
  "@odata.type": "#microsoft.graph.organization",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:00:52.2191086+03:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "57dd67da-67da-57dd-da67-dd57da67dd57"
    }
  ],
  "businessPhones": [
    "Business Phones value"
  ],
  "city": "City value",
  "country": "Country value",
  "countryLetterCode": "Country Letter Code value",
  "creationType": "Creation Type value",
  "displayName": "Display Name value",
  "marketingNotificationEmails": [
    "Marketing Notification Emails value"
  ],
  "onPremisesLastSyncDateTime": "2017-01-01T00:03:13.2795175+03:00",
  "onPremisesSyncEnabled": true,
  "postalCode": "Postal Code value",
  "preferredLanguage": "Preferred Language value",
  "privacyProfile": {
    "@odata.type": "microsoft.graph.privacyProfile",
    "contactEmail": "Contact Email value",
    "statementUrl": "https://example.com/statementUrl/"
  },
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan",
      "provisioningStatus": "Provisioning Status value"
    }
  ],
  "securityComplianceNotificationMails": [
    "Security Compliance Notification Mails value"
  ],
  "securityComplianceNotificationPhones": [
    "Security Compliance Notification Phones value"
  ],
  "state": "State value",
  "street": "Street value",
  "technicalNotificationMails": [
    "Technical Notification Mails value"
  ],
  "verifiedDomains": [
    {
      "@odata.type": "microsoft.graph.verifiedDomain",
      "capabilities": "Capabilities value",
      "isDefault": true,
      "isInitial": true,
      "name": "Name value",
      "type": "Type value"
    }
  ],
  "mobileDeviceManagementAuthority": "String"
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
Content-Length: 2051

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "305b9166-9166-305b-6691-5b3066915b30",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:00:52.2191086+03:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "57dd67da-67da-57dd-da67-dd57da67dd57"
    }
  ],
  "businessPhones": [
    "Business Phones value"
  ],
  "city": "City value",
  "country": "Country value",
  "countryLetterCode": "Country Letter Code value",
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "creationType": "Creation Type value",
  "displayName": "Display Name value",
  "marketingNotificationEmails": [
    "Marketing Notification Emails value"
  ],
  "onPremisesLastSyncDateTime": "2017-01-01T00:03:13.2795175+03:00",
  "onPremisesSyncEnabled": true,
  "postalCode": "Postal Code value",
  "preferredLanguage": "Preferred Language value",
  "privacyProfile": {
    "@odata.type": "microsoft.graph.privacyProfile",
    "contactEmail": "Contact Email value",
    "statementUrl": "https://example.com/statementUrl/"
  },
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan",
      "provisioningStatus": "Provisioning Status value"
    }
  ],
  "securityComplianceNotificationMails": [
    "Security Compliance Notification Mails value"
  ],
  "securityComplianceNotificationPhones": [
    "Security Compliance Notification Phones value"
  ],
  "state": "State value",
  "street": "Street value",
  "technicalNotificationMails": [
    "Technical Notification Mails value"
  ],
  "verifiedDomains": [
    {
      "@odata.type": "microsoft.graph.verifiedDomain",
      "capabilities": "Capabilities value",
      "isDefault": true,
      "isInitial": true,
      "name": "Name value",
      "type": "Type value"
    }
  ],
  "mobileDeviceManagementAuthority": "String"
}
```

