---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: acb2cd61442d1128756dba387e550088196cc36c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721740"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *listItemList = [[NSMutableArray alloc] init];
        listItemList = [jsonFinal valueForKey:@"value"];
        MSGraphListItem *listItem = [[MSGraphListItem alloc] initWithDictionary:[listItemList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```