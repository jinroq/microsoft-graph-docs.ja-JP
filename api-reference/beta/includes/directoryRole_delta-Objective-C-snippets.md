---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 488d88a3fa35999d3921d7f062bb4a688b1bccb4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35333905"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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