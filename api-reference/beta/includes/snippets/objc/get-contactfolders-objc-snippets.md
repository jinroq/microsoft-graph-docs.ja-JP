---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3f37272b3190f678b050a05a2f0e70cdac2be478
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527352"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contactFolders"]]];
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