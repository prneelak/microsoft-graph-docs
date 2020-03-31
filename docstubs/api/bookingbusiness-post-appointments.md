---
title: "Add appointments"
description: "Add appointments by posting to the appointments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add appointments

Namespace: microsoft.graph

Add appointments by posting to the appointments collection.

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
POST /bookingBusinesses/{bookingBusinessesId}/appointments/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [bookingAppointment](../resources/bookingappointment.md) object.

The following table shows the properties that are required when you create the [bookingAppointment](../resources/bookingappointment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|selfServiceAppointmentId|String||
|customerId|String||
|customerName|String||
|customerEmailAddress|String||
|customerPhone|String||
|customerLocation|[location](../resources/location.md)||
|customerNotes|String||
|serviceId|String||
|serviceName|String||
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|duration|Duration||
|preBuffer|Duration||
|postBuffer|Duration||
|serviceLocation|[location](../resources/location.md)||
|priceType|Enumeration| Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|price|Double||
|serviceNotes|String||
|reminders|[bookingReminder](../resources/bookingreminder.md) collection||
|optOutOfCustomerEmail|Boolean||
|staffMemberIds|String collection||
|invoiceAmount|Double||
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|invoiceId|String||
|invoiceStatus|Enumeration| Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [bookingAppointment](../resources/bookingappointment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_bookingappointment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/appointments
Content-type: application/json
Content-length: 2351

{
  "@odata.type": "#microsoft.graph.bookingAppointment",
  "selfServiceAppointmentId": "Self Service Appointment Id value",
  "customerId": "Customer Id value",
  "customerName": "Customer Name value",
  "customerEmailAddress": "Customer Email Address value",
  "customerPhone": "Customer Phone value",
  "customerLocation": {
    "@odata.type": "microsoft.graph.location",
    "displayName": "Display Name value",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "type": "String",
      "postOfficeBox": "Post Office Box value",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationUri": "Location Uri value",
    "locationType": "String",
    "uniqueId": "Unique Id value",
    "uniqueIdType": "String"
  },
  "customerNotes": "Customer Notes value",
  "serviceId": "Service Id value",
  "serviceName": "Service Name value",
  "start": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "Date Time value",
    "timeZone": "Time Zone value"
  },
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "duration": "PT49.1408484S",
  "preBuffer": "-PT1M47.5203165S",
  "postBuffer": "-PT23.3579744S",
  "serviceLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "priceType": "String",
  "price": "Double",
  "serviceNotes": "Service Notes value",
  "reminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder",
      "offset": "-PT1M18.3350919S",
      "recipients": "String",
      "message": "Message value"
    }
  ],
  "optOutOfCustomerEmail": true,
  "staffMemberIds": [
    "Staff Member Ids value"
  ],
  "invoiceAmount": "Double",
  "invoiceDate": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "invoiceId": "Invoice Id value",
  "invoiceStatus": "String",
  "invoiceUrl": "https://example.com/invoiceUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingappointment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2400

{
  "@odata.type": "#microsoft.graph.bookingAppointment",
  "id": "ece62ba4-2ba4-ece6-a42b-e6eca42be6ec",
  "selfServiceAppointmentId": "Self Service Appointment Id value",
  "customerId": "Customer Id value",
  "customerName": "Customer Name value",
  "customerEmailAddress": "Customer Email Address value",
  "customerPhone": "Customer Phone value",
  "customerLocation": {
    "@odata.type": "microsoft.graph.location",
    "displayName": "Display Name value",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "type": "String",
      "postOfficeBox": "Post Office Box value",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationUri": "Location Uri value",
    "locationType": "String",
    "uniqueId": "Unique Id value",
    "uniqueIdType": "String"
  },
  "customerNotes": "Customer Notes value",
  "serviceId": "Service Id value",
  "serviceName": "Service Name value",
  "start": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "Date Time value",
    "timeZone": "Time Zone value"
  },
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "duration": "PT49.1408484S",
  "preBuffer": "-PT1M47.5203165S",
  "postBuffer": "-PT23.3579744S",
  "serviceLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "priceType": "String",
  "price": "Double",
  "serviceNotes": "Service Notes value",
  "reminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder",
      "offset": "-PT1M18.3350919S",
      "recipients": "String",
      "message": "Message value"
    }
  ],
  "optOutOfCustomerEmail": true,
  "staffMemberIds": [
    "Staff Member Ids value"
  ],
  "invoiceAmount": "Double",
  "invoiceDate": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "invoiceId": "Invoice Id value",
  "invoiceStatus": "String",
  "invoiceUrl": "https://example.com/invoiceUrl/"
}
```

