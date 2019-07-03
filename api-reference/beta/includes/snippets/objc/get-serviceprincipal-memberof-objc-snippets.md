---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 21cec39df08ea22fd4e8d0033c2a5f4f5b95d4d4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526958"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/memberOf"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *directoryObjectList = [[NSMutableArray alloc] init];
        directoryObjectList = [jsonFinal valueForKey:@"value"];
        MSGraphDirectoryObject *directoryObject = [[MSGraphDirectoryObject alloc] initWithDictionary:[directoryObjectList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```