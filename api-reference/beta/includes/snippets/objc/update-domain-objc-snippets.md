---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 61fa32f93968ae41e76f7fd5c7403a2de9d86376
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485151"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/domains/contoso.com"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDomain *domain = [[MSGraphDomain alloc] init];
[domain setIsDefault: true];
NSMutableArray *supportedServicesList = [[NSMutableArray alloc] init];
[supportedServicesList addObject: @"Email"];
[supportedServicesList addObject: @"OfficeCommunicationsOnline"];
[domain setSupportedServices:supportedServicesList];

NSError *error;
NSData *domainData = [domain getSerializedDataWithError:&error];
[urlRequest setHTTPBody:domainData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```