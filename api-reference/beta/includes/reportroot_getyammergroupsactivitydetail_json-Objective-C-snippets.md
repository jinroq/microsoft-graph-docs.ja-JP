---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 30824fd7b34e5c3230b90a5dde7ebfb5bcdcecc8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35333969"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *yammerGroupsActivityDetailList = [[NSMutableArray alloc] init];
        yammerGroupsActivityDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphYammerGroupsActivityDetail *yammerGroupsActivityDetail = [[MSGraphYammerGroupsActivityDetail alloc] initWithDictionary:[yammerGroupsActivityDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```