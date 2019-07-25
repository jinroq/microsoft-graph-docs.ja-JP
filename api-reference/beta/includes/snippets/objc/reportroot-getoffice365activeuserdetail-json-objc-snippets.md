---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 253758f714d3cf5a5be27bdd6080746e47e4d952
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719338"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365ActiveUserDetailList = [[NSMutableArray alloc] init];
        office365ActiveUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365ActiveUserDetail *office365ActiveUserDetail = [[MSGraphOffice365ActiveUserDetail alloc] initWithDictionary:[office365ActiveUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```