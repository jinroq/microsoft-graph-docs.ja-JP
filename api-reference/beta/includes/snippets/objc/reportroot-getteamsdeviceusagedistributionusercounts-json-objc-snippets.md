---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 89a8e41cb4a2e6022d7a4b9dd60dfa6681cbd6f6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718605"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *teamsDeviceUsageDistributionUserCountsList = [[NSMutableArray alloc] init];
        teamsDeviceUsageDistributionUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphTeamsDeviceUsageDistributionUserCounts *teamsDeviceUsageDistributionUserCounts = [[MSGraphTeamsDeviceUsageDistributionUserCounts alloc] initWithDictionary:[teamsDeviceUsageDistributionUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```