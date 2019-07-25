---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4dbeae6a23eb12d63ca0b807817bd2b0c820010f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719278"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365ServicesUserCountsList = [[NSMutableArray alloc] init];
        office365ServicesUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365ServicesUserCounts *office365ServicesUserCounts = [[MSGraphOffice365ServicesUserCounts alloc] initWithDictionary:[office365ServicesUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```