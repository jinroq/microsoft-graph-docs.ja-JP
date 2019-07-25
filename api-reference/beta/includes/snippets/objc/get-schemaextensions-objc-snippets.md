---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a58acbbbfe4910495caa6039e0c1b573fe4624a5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718065"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/schemaExtensions?$filter=id%20eq%20'graphlearn_test'"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *schemaExtensionList = [[NSMutableArray alloc] init];
        schemaExtensionList = [jsonFinal valueForKey:@"value"];
        MSGraphSchemaExtension *schemaExtension = [[MSGraphSchemaExtension alloc] initWithDictionary:[schemaExtensionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```