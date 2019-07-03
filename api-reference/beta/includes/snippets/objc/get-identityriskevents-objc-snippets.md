---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dfcffe1451a3072656bd8638c1f92e66cd7d6a4d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487070"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityRiskEvents"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *identityRiskEventList = [[NSMutableArray alloc] init];
        identityRiskEventList = [jsonFinal valueForKey:@"value"];
        MSGraphIdentityRiskEvent *identityRiskEvent = [[MSGraphIdentityRiskEvent alloc] initWithDictionary:[identityRiskEventList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```