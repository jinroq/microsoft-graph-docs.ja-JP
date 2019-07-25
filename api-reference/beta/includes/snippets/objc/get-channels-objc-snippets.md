---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2ecfde9af24d41cf066f0b55950e4667e5353e4f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708626"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/channels"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *channelList = [[NSMutableArray alloc] init];
        channelList = [jsonFinal valueForKey:@"value"];
        MSGraphChannel *channel = [[MSGraphChannel alloc] initWithDictionary:[channelList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```