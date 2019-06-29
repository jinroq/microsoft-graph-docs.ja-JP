---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a63b9df317109c9b44a836b62b86944875271f5e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35316080"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/securityActions"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *securityActionList = [[NSMutableArray alloc] init];
        securityActionList = [jsonFinal valueForKey:@"value"];
        MSGraphSecurityAction *securityAction = [[MSGraphSecurityAction alloc] initWithDictionary:[securityActionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```