---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6ff6a33b69720d4c0dc1a4813c787311756f1283
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35326028"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/subscriptions"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *subscriptionList = [[NSMutableArray alloc] init];
        subscriptionList = [jsonFinal valueForKey:@"value"];
        MSGraphSubscription *subscription = [[MSGraphSubscription alloc] initWithDictionary:[subscriptionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```