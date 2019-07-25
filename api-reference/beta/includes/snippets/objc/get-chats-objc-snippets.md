---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5eaaae1108bcacc9e5ee0b14d1710101fe2760fb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707740"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{id}/chats"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *chatList = [[NSMutableArray alloc] init];
        chatList = [jsonFinal valueForKey:@"value"];
        MSGraphChat *chat = [[MSGraphChat alloc] initWithDictionary:[chatList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```