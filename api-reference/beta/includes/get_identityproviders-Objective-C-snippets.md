---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bcdec765f996d206b94795c6e5258923006f9904
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334331"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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