---
title: "Create users"
description: "Create users by posting to the users collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create users

Namespace: microsoft.graph

Create users by posting to the users collection.

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
POST /education/classes/{educationClassId}/schools/{educationSchoolId}/users/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [educationUser](../resources/educationuser.md) object.

The following table shows the properties that are required when you create the [educationUser](../resources/educationuser.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|primaryRole|Enumeration|. Possible values are: `student`, `teacher`, `none`, `unknownFutureValue`.|
|middleName|String||
|externalSource|Enumeration|. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|residenceAddress|[physicalAddress](../resources/physicaladdress.md)||
|mailingAddress|[physicalAddress](../resources/physicaladdress.md)||
|student|[educationStudent](../resources/educationstudent.md)||
|teacher|[educationTeacher](../resources/educationteacher.md)||
|createdBy|[identitySet](../resources/identityset.md)||
|accountEnabled|Boolean||
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection||
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection||
|businessPhones|String collection||
|department|String||
|displayName|String||
|givenName|String||
|mail|String||
|mailNickname|String||
|mobilePhone|String||
|passwordPolicies|String||
|passwordProfile|[passwordProfile](../resources/passwordprofile.md)||
|officeLocation|String||
|preferredLanguage|String||
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection||
|refreshTokensValidFromDateTime|DateTimeOffset||
|showInAddressList|Boolean||
|surname|String||
|usageLocation|String||
|userPrincipalName|String||
|userType|String||



## Response
If successful, this method returns a `201 Created` response code and a [educationUser](../resources/educationuser.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/education/classes/{educationClassId}/schools/{educationSchoolId}/users
Content-type: application/json
Content-length: 2925

{
  "@odata.type": "#microsoft.graph.educationUser",
  "primaryRole": "String",
  "middleName": "Middle Name value",
  "externalSource": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent",
    "graduationYear": "Graduation Year value",
    "grade": "Grade value",
    "birthDate": "Date",
    "gender": "String",
    "studentNumber": "Student Number value",
    "externalId": "External Id value"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher",
    "teacherNumber": "Teacher Number value"
  },
  "createdBy": {
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
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "c5ceb44e-b44e-c5ce-4eb4-cec54eb4cec5"
      ],
      "skuId": "463dfbb4-fbb4-463d-b4fb-3d46b4fb3d46"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:03:31.5255847+03:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "0ac114bc-14bc-0ac1-bc14-c10abc14c10a"
    }
  ],
  "businessPhones": [
    "Business Phones value"
  ],
  "department": "Department value",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "mail": "Mail value",
  "mailNickname": "Mail Nickname value",
  "mobilePhone": "Mobile Phone value",
  "passwordPolicies": "Password Policies value",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile",
    "password": "Password value",
    "forceChangePasswordNextSignIn": true,
    "forceChangePasswordNextSignInWithMfa": true
  },
  "officeLocation": "Office Location value",
  "preferredLanguage": "Preferred Language value",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan",
      "provisioningStatus": "Provisioning Status value"
    }
  ],
  "refreshTokensValidFromDateTime": "2017-01-01T00:02:30.9564271+03:00",
  "showInAddressList": true,
  "surname": "Surname value",
  "usageLocation": "Usage Location value",
  "userPrincipalName": "User Principal Name value",
  "userType": "User Type value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationuser"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2974

{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "7d0431c3-31c3-7d04-c331-047dc331047d",
  "primaryRole": "String",
  "middleName": "Middle Name value",
  "externalSource": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent",
    "graduationYear": "Graduation Year value",
    "grade": "Grade value",
    "birthDate": "Date",
    "gender": "String",
    "studentNumber": "Student Number value",
    "externalId": "External Id value"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher",
    "teacherNumber": "Teacher Number value"
  },
  "createdBy": {
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
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "c5ceb44e-b44e-c5ce-4eb4-cec54eb4cec5"
      ],
      "skuId": "463dfbb4-fbb4-463d-b4fb-3d46b4fb3d46"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:03:31.5255847+03:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "0ac114bc-14bc-0ac1-bc14-c10abc14c10a"
    }
  ],
  "businessPhones": [
    "Business Phones value"
  ],
  "department": "Department value",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "mail": "Mail value",
  "mailNickname": "Mail Nickname value",
  "mobilePhone": "Mobile Phone value",
  "passwordPolicies": "Password Policies value",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile",
    "password": "Password value",
    "forceChangePasswordNextSignIn": true,
    "forceChangePasswordNextSignInWithMfa": true
  },
  "officeLocation": "Office Location value",
  "preferredLanguage": "Preferred Language value",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan",
      "provisioningStatus": "Provisioning Status value"
    }
  ],
  "refreshTokensValidFromDateTime": "2017-01-01T00:02:30.9564271+03:00",
  "showInAddressList": true,
  "surname": "Surname value",
  "usageLocation": "Usage Location value",
  "userPrincipalName": "User Principal Name value",
  "userType": "User Type value"
}
```

