---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c987f3f17b03692cc330c8526c0cfd6feb80e153
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736539"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityProviders"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *identityProviderList = [[NSMutableArray alloc] init];
        identityProviderList = [jsonFinal valueForKey:@"value"];
        MSGraphIdentityProvider *identityProvider = [[MSGraphIdentityProvider alloc] initWithDictionary:[identityProviderList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```