---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e4d0e403332eccb9ff9c159df8287e9d11898f14
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723386"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/auditLogs/provisioning"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *provisioningObjectSummaryList = [[NSMutableArray alloc] init];
        provisioningObjectSummaryList = [jsonFinal valueForKey:@"value"];
        MSGraphProvisioningObjectSummary *provisioningObjectSummary = [[MSGraphProvisioningObjectSummary alloc] initWithDictionary:[provisioningObjectSummaryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```