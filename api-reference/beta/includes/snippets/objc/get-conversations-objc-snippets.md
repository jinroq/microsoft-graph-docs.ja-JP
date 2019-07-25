---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c3987495c751d1d4327f0fd8deb2d1e297f6cbe4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713690"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/conversations"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *conversationList = [[NSMutableArray alloc] init];
        conversationList = [jsonFinal valueForKey:@"value"];
        MSGraphConversation *conversation = [[MSGraphConversation alloc] initWithDictionary:[conversationList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```