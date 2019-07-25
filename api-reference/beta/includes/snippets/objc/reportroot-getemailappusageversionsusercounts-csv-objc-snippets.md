---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: efcac655dae7126be497be21db662a2afde3d15e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727616"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAppUsageVersionsUserCountsList = [[NSMutableArray alloc] init];
        emailAppUsageVersionsUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAppUsageVersionsUserCounts *emailAppUsageVersionsUserCounts = [[MSGraphEmailAppUsageVersionsUserCounts alloc] initWithDictionary:[emailAppUsageVersionsUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```