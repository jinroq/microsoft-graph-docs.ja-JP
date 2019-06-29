---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9a8ef17a8ac2d8777c28eb053f958dd0ee152fc6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35333757"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365GroupsActivityGroupCountsList = [[NSMutableArray alloc] init];
        office365GroupsActivityGroupCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365GroupsActivityGroupCounts *office365GroupsActivityGroupCounts = [[MSGraphOffice365GroupsActivityGroupCounts alloc] initWithDictionary:[office365GroupsActivityGroupCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```