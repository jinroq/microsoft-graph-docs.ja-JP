---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1e199c9e6af3b12774a9f0641c84ddd965c62f9d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718941"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessActivityUserCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessActivityUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessActivityUserCounts *skypeForBusinessActivityUserCounts = [[MSGraphSkypeForBusinessActivityUserCounts alloc] initWithDictionary:[skypeForBusinessActivityUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```