---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 05ebbb59d4d3387f5e13e5a57a6b8f277fa25d6f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715728"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/subscribedSkus"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *subscribedSkuList = [[NSMutableArray alloc] init];
        subscribedSkuList = [jsonFinal valueForKey:@"value"];
        MSGraphSubscribedSku *subscribedSku = [[MSGraphSubscribedSku alloc] initWithDictionary:[subscribedSkuList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```