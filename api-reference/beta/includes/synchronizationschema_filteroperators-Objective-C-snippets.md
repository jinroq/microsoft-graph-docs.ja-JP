---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dfc6877c7cd834a3526d4bdd8475ced575f15a58
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35333573"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *filterOperatorSchemaList = [[NSMutableArray alloc] init];
        filterOperatorSchemaList = [jsonFinal valueForKey:@"value"];
        MSGraphFilterOperatorSchema *filterOperatorSchema = [[MSGraphFilterOperatorSchema alloc] initWithDictionary:[filterOperatorSchemaList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```