---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 23c4de516564c48267e054634cc3996d03c21088
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719638"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAppUsageUserDetailList = [[NSMutableArray alloc] init];
        emailAppUsageUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAppUsageUserDetail *emailAppUsageUserDetail = [[MSGraphEmailAppUsageUserDetail alloc] initWithDictionary:[emailAppUsageUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```