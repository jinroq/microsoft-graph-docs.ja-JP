---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 60d4b02a364b37e51f84bc0447ad7fee54d73840
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718292"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/riskyUsers"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *riskyUserList = [[NSMutableArray alloc] init];
        riskyUserList = [jsonFinal valueForKey:@"value"];
        MSGraphRiskyUser *riskyUser = [[MSGraphRiskyUser alloc] initWithDictionary:[riskyUserList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```