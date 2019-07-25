---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 654906553d9eb9c9487bcea4a001554d4b2c20a8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728254"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/programControlTypes"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *programControlTypeList = [[NSMutableArray alloc] init];
        programControlTypeList = [jsonFinal valueForKey:@"value"];
        MSGraphProgramControlType *programControlType = [[MSGraphProgramControlType alloc] initWithDictionary:[programControlTypeList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```