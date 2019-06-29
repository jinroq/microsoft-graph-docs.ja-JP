---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e87948c07877ad5d08354127dcb2468be9d0127e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334069"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/contacts"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *orgContactList = [[NSMutableArray alloc] init];
        orgContactList = [jsonFinal valueForKey:@"value"];
        MSGraphOrgContact *orgContact = [[MSGraphOrgContact alloc] initWithDictionary:[orgContactList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```