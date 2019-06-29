---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 078a44ac8f85a5a035d7c91e665b70fcae641c7b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334250"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/agreements"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *agreementList = [[NSMutableArray alloc] init];
        agreementList = [jsonFinal valueForKey:@"value"];
        MSGraphAgreement *agreement = [[MSGraphAgreement alloc] initWithDictionary:[agreementList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```