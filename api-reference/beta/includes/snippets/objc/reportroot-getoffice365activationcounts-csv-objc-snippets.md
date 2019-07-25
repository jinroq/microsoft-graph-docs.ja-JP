---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d9c3021cfad49b239df7316e890e7acaf382e814
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719484"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ActivationCounts?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365ActivationCountsList = [[NSMutableArray alloc] init];
        office365ActivationCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365ActivationCounts *office365ActivationCounts = [[MSGraphOffice365ActivationCounts alloc] initWithDictionary:[office365ActivationCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```