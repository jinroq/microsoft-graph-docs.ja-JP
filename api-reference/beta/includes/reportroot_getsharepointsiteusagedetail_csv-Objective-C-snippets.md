---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2d507e417dec64e98155c101b2472f1297fc1d69
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334290"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointSiteUsageDetailList = [[NSMutableArray alloc] init];
        sharePointSiteUsageDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointSiteUsageDetail *sharePointSiteUsageDetail = [[MSGraphSharePointSiteUsageDetail alloc] initWithDictionary:[sharePointSiteUsageDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```