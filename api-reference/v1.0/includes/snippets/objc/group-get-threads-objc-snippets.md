---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 515c3ec6fe44a4fe324679c19cb33fa7bfcce4c4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888184"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/threads"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *conversationThreadList = [[NSMutableArray alloc] init];
        conversationThreadList = [jsonFinal valueForKey:@"value"];
        MSGraphConversationThread *conversationThread = [[MSGraphConversationThread alloc] initWithDictionary:[conversationThreadList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```