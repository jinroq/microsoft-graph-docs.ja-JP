---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 830a2f7ba60b78d0821c00540403c2e8b57d2bf5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334602"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365GroupsActivityCountsList = [[NSMutableArray alloc] init];
        office365GroupsActivityCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365GroupsActivityCounts *office365GroupsActivityCounts = [[MSGraphOffice365GroupsActivityCounts alloc] initWithDictionary:[office365GroupsActivityCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```