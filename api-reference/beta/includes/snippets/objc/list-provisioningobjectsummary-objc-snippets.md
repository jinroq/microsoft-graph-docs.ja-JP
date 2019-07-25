---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e4255edf3ff97d02dac7f0de09e1a91cb99091a1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720010"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/auditLogs/directoryProvisioning"]]];
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