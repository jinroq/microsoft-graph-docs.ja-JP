---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b51a2caff89b09c0bdd792a21866a49412837168
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734090"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/auditLogs/signIns"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *signInList = [[NSMutableArray alloc] init];
        signInList = [jsonFinal valueForKey:@"value"];
        MSGraphSignIn *signIn = [[MSGraphSignIn alloc] initWithDictionary:[signInList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```