---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1bbdfbc0a12ae3ab77376e87185d969b7b831e76
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883893"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contactFolders/{id}/contacts"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *contactList = [[NSMutableArray alloc] init];
        contactList = [jsonFinal valueForKey:@"value"];
        MSGraphContact *contact = [[MSGraphContact alloc] initWithDictionary:[contactList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```