---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2989f9b3edeabeafb58ed2ef194020feb5829a23
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35325344"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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