---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f322addb10eca2516eace042e9c787aeafd40873
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734021"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directoryRoles/delta"]]];
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