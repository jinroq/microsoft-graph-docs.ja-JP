---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e4d43b54cf85df7393b5ea9dd0bf8930d47047d2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334555"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *yammerDeviceUsageDistributionUserCountsList = [[NSMutableArray alloc] init];
        yammerDeviceUsageDistributionUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphYammerDeviceUsageDistributionUserCounts *yammerDeviceUsageDistributionUserCounts = [[MSGraphYammerDeviceUsageDistributionUserCounts alloc] initWithDictionary:[yammerDeviceUsageDistributionUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```