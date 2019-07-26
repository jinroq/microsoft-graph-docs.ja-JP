---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 0b43fbd810ebae87f95835e116871728e750349c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880766"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/calendars"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *calendarList = [[NSMutableArray alloc] init];
        calendarList = [jsonFinal valueForKey:@"value"];
        MSGraphCalendar *calendar = [[MSGraphCalendar alloc] initWithDictionary:[calendarList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```