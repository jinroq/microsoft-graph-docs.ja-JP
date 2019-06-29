---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2acb36a754fcea094b50f146dba5ec9f77a49cc1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35320157"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedAccess/azureResources/resources"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *governanceResourceList = [[NSMutableArray alloc] init];
        governanceResourceList = [jsonFinal valueForKey:@"value"];
        MSGraphGovernanceResource *governanceResource = [[MSGraphGovernanceResource alloc] initWithDictionary:[governanceResourceList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```