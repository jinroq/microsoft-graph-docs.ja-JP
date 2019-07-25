---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c4e3b6cc2f390170ba62dcc9ab9fb3d82a7d96a5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719695"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailActivityUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailActivitySummaryList = [[NSMutableArray alloc] init];
        emailActivitySummaryList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailActivitySummary *emailActivitySummary = [[MSGraphEmailActivitySummary alloc] initWithDictionary:[emailActivitySummaryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```