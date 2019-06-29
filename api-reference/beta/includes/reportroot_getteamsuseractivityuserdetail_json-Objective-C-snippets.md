---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dde0b6344cb923d59dec76f0e31707ce3b3216d0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35316048"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *teamsUserActivityUserDetailList = [[NSMutableArray alloc] init];
        teamsUserActivityUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphTeamsUserActivityUserDetail *teamsUserActivityUserDetail = [[MSGraphTeamsUserActivityUserDetail alloc] initWithDictionary:[teamsUserActivityUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```