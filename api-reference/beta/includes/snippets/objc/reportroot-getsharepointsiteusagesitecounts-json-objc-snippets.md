---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 64cc8c5a10be220620d545f2e2066cd6cd02b88c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726982"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointSiteUsageSiteCountsList = [[NSMutableArray alloc] init];
        sharePointSiteUsageSiteCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointSiteUsageSiteCounts *sharePointSiteUsageSiteCounts = [[MSGraphSharePointSiteUsageSiteCounts alloc] initWithDictionary:[sharePointSiteUsageSiteCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```