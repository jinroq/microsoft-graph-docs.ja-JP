---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1c512f83830fc077c1ae4fb9fff5c03fb664a7a5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719487"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ActivationCounts?$format=application/json"]]];
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