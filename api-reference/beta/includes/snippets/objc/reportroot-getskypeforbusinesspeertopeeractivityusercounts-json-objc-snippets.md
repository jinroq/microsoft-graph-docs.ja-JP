---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4f2d1f1902abf49de285070bab4da99c5198034f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485544"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessPeerToPeerActivityUserCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessPeerToPeerActivityUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessPeerToPeerActivityUserCounts *skypeForBusinessPeerToPeerActivityUserCounts = [[MSGraphSkypeForBusinessPeerToPeerActivityUserCounts alloc] initWithDictionary:[skypeForBusinessPeerToPeerActivityUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```