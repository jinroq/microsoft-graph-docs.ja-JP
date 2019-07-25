---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fac97b31c4c24dfd4079f0254627eb4c2ea9b00c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709742"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *bookingCustomerList = [[NSMutableArray alloc] init];
        bookingCustomerList = [jsonFinal valueForKey:@"value"];
        MSGraphBookingCustomer *bookingCustomer = [[MSGraphBookingCustomer alloc] initWithDictionary:[bookingCustomerList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```