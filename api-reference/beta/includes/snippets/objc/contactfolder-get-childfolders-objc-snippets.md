---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 57e7550d83f2a4d2ff43d281483665405cac5143
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863265"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contactFolders/{id}/childFolders"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *contactFolderList = [[NSMutableArray alloc] init];
        contactFolderList = [jsonFinal valueForKey:@"value"];
        MSGraphContactFolder *contactFolder = [[MSGraphContactFolder alloc] initWithDictionary:[contactFolderList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```