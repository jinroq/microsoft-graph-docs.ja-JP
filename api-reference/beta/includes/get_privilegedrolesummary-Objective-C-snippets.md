---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c618de2dbe8fc23c1f0cbf56bc1cc40d17056481
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35316135"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedRoles/{id}/summary"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPrivilegedRoleSummary *privilegedRoleSummary = [[MSGraphPrivilegedRoleSummary alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```