---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: f41846f8d3d37d8b98db9a1559ceff4fc362ad11
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932102"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/calendar/getschedule"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"outlook.timezone=\"Pacific Standard Time\"" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *schedulesList = [[NSMutableArray alloc] init];
[schedulesList addObject: @"adelev@contoso.onmicrosoft.com"];
[schedulesList addObject: @"meganb@contoso.onmicrosoft.com"];
payloadDictionary[@"schedules"] = schedulesList;

MSGraphDateTimeTimeZone *startTime = [[MSGraphDateTimeTimeZone alloc] init];
[startTime setDateTime: "2019-03-15T09:00:00"];
[startTime setTimeZone:@"Pacific Standard Time"];
payloadDictionary[@"startTime"] = startTime;

MSGraphDateTimeTimeZone *endTime = [[MSGraphDateTimeTimeZone alloc] init];
[endTime setDateTime: "2019-03-15T18:00:00"];
[endTime setTimeZone:@"Pacific Standard Time"];
payloadDictionary[@"endTime"] = endTime;

NSString *availabilityViewInterval = @"60";
payloadDictionary[@"availabilityViewInterval"] = availabilityViewInterval;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```