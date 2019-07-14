---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1d698317114a610e72ccb6b01556205dd3f316fb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527277"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getAzureADApplicationSignInSummary(period='D7')"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *applicationSignInSummaryList = [[NSMutableArray alloc] init];
        applicationSignInSummaryList = [jsonFinal valueForKey:@"value"];
        MSGraphApplicationSignInSummary *applicationSignInSummary = [[MSGraphApplicationSignInSummary alloc] initWithDictionary:[applicationSignInSummaryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```