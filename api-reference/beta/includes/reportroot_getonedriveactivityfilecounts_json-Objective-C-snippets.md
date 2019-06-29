---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8025766dbf582f59bdcb7dea41fb08d8cf80d72a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35333577"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveActivityFileCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *siteActivitySummaryList = [[NSMutableArray alloc] init];
        siteActivitySummaryList = [jsonFinal valueForKey:@"value"];
        MSGraphSiteActivitySummary *siteActivitySummary = [[MSGraphSiteActivitySummary alloc] initWithDictionary:[siteActivitySummaryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```