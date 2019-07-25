---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dcd10a740ead42e8b1cbae8d8e1a510ca185343e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709519"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphBookingService *bookingService = [[MSGraphBookingService alloc] init];
[bookingService setDefaultDuration:@"PT1H30M"];
MSGraphLocation *defaultLocation = [[MSGraphLocation alloc] init];
MSGraphPhysicalAddress *address = [[MSGraphPhysicalAddress alloc] init];
[address setCity:@"Buffalo"];
[address setCountryOrRegion:@"USA"];
[address setPostalCode:@"98052"];
[address setPostOfficeBox: null];
[address setState:@"NY"];
[address setStreet:@"4567 First Street"];
[address setType: null];
[defaultLocation setAddress:address];
[defaultLocation setCoordinates: null];
[defaultLocation setDisplayName:@"Contoso Lunch Delivery"];
[defaultLocation setLocationEmailAddress: null];
[defaultLocation setLocationType: null];
[defaultLocation setLocationUri: null];
[defaultLocation setUniqueId: null];
[defaultLocation setUniqueIdType: null];
[bookingService setDefaultLocation:defaultLocation];
[bookingService setDefaultPrice: 10.0];
[bookingService setDefaultPriceType: [MSGraphBookingPriceType fixedPrice]];
NSMutableArray *defaultRemindersList = [[NSMutableArray alloc] init];
MSGraphBookingReminder *defaultReminders = [[MSGraphBookingReminder alloc] init];
[defaultReminders setMessage:@"Please be reminded that this service is tomorrow."];
[defaultReminders setOffset:@"P1D"];
[defaultReminders setRecipients: [MSGraphBookingReminderRecipients allAttendees]];
[defaultRemindersList addObject: defaultReminders];
[bookingService setDefaultReminders:defaultRemindersList];
[bookingService setDescription:@"Individual bento box lunch delivery"];
[bookingService setDisplayName:@"Bento"];
[bookingService setIsHiddenFromCustomers: false];
[bookingService setNotes:@"Home-cooked special"];
[bookingService setPostBuffer:@"PT10M"];
[bookingService setPreBuffer:@"PT5M"];
MSGraphBookingSchedulingPolicy *schedulingPolicy = [[MSGraphBookingSchedulingPolicy alloc] init];
[schedulingPolicy setAllowStaffSelection: true];
[schedulingPolicy setMaximumAdvance:@"P10D"];
[schedulingPolicy setMinimumLeadTime:@"PT10H"];
[schedulingPolicy setSendConfirmationsToOwner: true];
[schedulingPolicy setTimeSlotInterval:@"PT1H"];
[bookingService setSchedulingPolicy:schedulingPolicy];
NSMutableArray *staffMemberIdsList = [[NSMutableArray alloc] init];
[staffMemberIdsList addObject: @"d90d1e8c-5cfe-48cf-a2d5-966267375b6a"];
[staffMemberIdsList addObject: @"2f5f8794-0b29-45b5-b56a-2eb5ff7aa880"];
[bookingService setStaffMemberIds:staffMemberIdsList];

NSError *error;
NSData *bookingServiceData = [bookingService getSerializedDataWithError:&error];
[urlRequest setHTTPBody:bookingServiceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```