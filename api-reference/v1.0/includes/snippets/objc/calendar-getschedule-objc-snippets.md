---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 53bed3f4a09ae4932eeab090dd568c7397e6106e
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396773"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/calendar/getSchedule"]]];
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

int32_t availabilityViewInterval = 60;
payloadDictionary[@"availabilityViewInterval"] = availabilityViewInterval;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```