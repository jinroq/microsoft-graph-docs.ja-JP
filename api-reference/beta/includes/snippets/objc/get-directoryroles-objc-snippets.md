---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0431a575bed7ebea1ab82379be97b0b545470b62
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713354"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directoryRoles"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *directoryRoleList = [[NSMutableArray alloc] init];
        directoryRoleList = [jsonFinal valueForKey:@"value"];
        MSGraphDirectoryRole *directoryRole = [[MSGraphDirectoryRole alloc] initWithDictionary:[directoryRoleList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```