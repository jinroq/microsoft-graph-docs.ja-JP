---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 21ea8670f442827e3a59d1d91f478a2076144e02
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710213"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/applicationSignInDetailedSummary/'id'"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphApplicationSignInDetailedSummary *applicationSignInDetailedSummary = [[MSGraphApplicationSignInDetailedSummary alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```