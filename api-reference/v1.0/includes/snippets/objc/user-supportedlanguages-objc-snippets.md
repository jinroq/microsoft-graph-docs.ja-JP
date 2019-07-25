---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d3a8b150db3f976783c8199f5f4543f30c8b251c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732952"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/supportedLanguages"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *localeInfoList = [[NSMutableArray alloc] init];
        localeInfoList = [jsonFinal valueForKey:@"value"];
        MSGraphLocaleInfo *localeInfo = [[MSGraphLocaleInfo alloc] initWithDictionary:[localeInfoList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```