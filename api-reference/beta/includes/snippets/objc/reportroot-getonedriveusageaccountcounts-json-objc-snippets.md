---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 830433708aa6ba8a294c0894a0fd909ff16b941f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719195"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *oneDriveUsageAccountCountsList = [[NSMutableArray alloc] init];
        oneDriveUsageAccountCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOneDriveUsageAccountCounts *oneDriveUsageAccountCounts = [[MSGraphOneDriveUsageAccountCounts alloc] initWithDictionary:[oneDriveUsageAccountCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```