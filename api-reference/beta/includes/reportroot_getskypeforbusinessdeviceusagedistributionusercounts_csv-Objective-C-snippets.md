---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 45c08b071818a80ba700425313b97f3046afd99c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334635"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessDeviceUsageDistributionUserCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessDeviceUsageDistributionUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessDeviceUsageDistributionUserCounts *skypeForBusinessDeviceUsageDistributionUserCounts = [[MSGraphSkypeForBusinessDeviceUsageDistributionUserCounts alloc] initWithDictionary:[skypeForBusinessDeviceUsageDistributionUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```