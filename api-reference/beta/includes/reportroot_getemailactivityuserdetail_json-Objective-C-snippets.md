---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 66b61537408a509707fa705b1c83d917c8fe5c0c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334657"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailActivityUserDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailActivityUserDetailList = [[NSMutableArray alloc] init];
        emailActivityUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailActivityUserDetail *emailActivityUserDetail = [[MSGraphEmailActivityUserDetail alloc] initWithDictionary:[emailActivityUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```