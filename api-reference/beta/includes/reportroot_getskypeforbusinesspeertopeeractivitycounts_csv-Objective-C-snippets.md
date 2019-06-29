---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cb2a44cba890b51ae937c48d4a49253eb20a0e18
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35333755"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessPeerToPeerActivityCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessPeerToPeerActivityCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessPeerToPeerActivityCounts *skypeForBusinessPeerToPeerActivityCounts = [[MSGraphSkypeForBusinessPeerToPeerActivityCounts alloc] initWithDictionary:[skypeForBusinessPeerToPeerActivityCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```