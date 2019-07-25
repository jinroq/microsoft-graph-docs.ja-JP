---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b9a1da8b42a7b37676e7bae287c93731e2159966
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718897"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointSiteUsagePages(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointSiteUsagePagesList = [[NSMutableArray alloc] init];
        sharePointSiteUsagePagesList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointSiteUsagePages *sharePointSiteUsagePages = [[MSGraphSharePointSiteUsagePages alloc] initWithDictionary:[sharePointSiteUsagePagesList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```