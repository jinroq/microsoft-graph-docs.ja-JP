---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: abb5ecde39418addb1c9501d831eccc7e432d219
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35333832"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessActivityCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessActivityCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessActivityCounts *skypeForBusinessActivityCounts = [[MSGraphSkypeForBusinessActivityCounts alloc] initWithDictionary:[skypeForBusinessActivityCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```