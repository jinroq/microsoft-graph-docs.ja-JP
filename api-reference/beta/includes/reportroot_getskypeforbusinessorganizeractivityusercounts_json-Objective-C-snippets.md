---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 49b2b48a7489e7c8878fb3da7b871219a4301d84
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334012"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessOrganizerActivityUserCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessOrganizerActivityUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessOrganizerActivityUserCounts *skypeForBusinessOrganizerActivityUserCounts = [[MSGraphSkypeForBusinessOrganizerActivityUserCounts alloc] initWithDictionary:[skypeForBusinessOrganizerActivityUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```