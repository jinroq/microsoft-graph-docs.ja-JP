---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d9b6c69817ddcfadfd31bb3891b1d9c3f06f8601
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709554"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingCurrencies"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *bookingCurrencyList = [[NSMutableArray alloc] init];
        bookingCurrencyList = [jsonFinal valueForKey:@"value"];
        MSGraphBookingCurrency *bookingCurrency = [[MSGraphBookingCurrency alloc] initWithDictionary:[bookingCurrencyList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```