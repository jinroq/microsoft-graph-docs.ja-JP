---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6dddf01ef37d62b93e0a2900f18f9de55288bc76
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721656"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailFolders/inbox/messagerules"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *messageRuleList = [[NSMutableArray alloc] init];
        messageRuleList = [jsonFinal valueForKey:@"value"];
        MSGraphMessageRule *messageRule = [[MSGraphMessageRule alloc] initWithDictionary:[messageRuleList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```