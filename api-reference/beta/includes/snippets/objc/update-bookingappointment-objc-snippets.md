---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0bf3317e5db80342a005ea755356386de19d500e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709917"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA="]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphBookingAppointment *bookingAppointment = [[MSGraphBookingAppointment alloc] init];
MSGraphDateTimeTimeZone *end = [[MSGraphDateTimeTimeZone alloc] init];
[end setDateTime: "2018-05-06T15:30:00+03:00"];
[end setTimeZone:@"UTC"];
[bookingAppointment setEnd:end];
MSGraphDateTimeTimeZone *invoiceDate = [[MSGraphDateTimeTimeZone alloc] init];
[invoiceDate setDateTime: "2018-05-06T15:30:00+03:00"];
[invoiceDate setTimeZone:@"UTC"];
[bookingAppointment setInvoiceDate:invoiceDate];
MSGraphDateTimeTimeZone *start = [[MSGraphDateTimeTimeZone alloc] init];
[start setDateTime: "2018-05-06T15:00:00+03:00"];
[start setTimeZone:@"UTC"];
[bookingAppointment setStart:start];

NSError *error;
NSData *bookingAppointmentData = [bookingAppointment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:bookingAppointmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```