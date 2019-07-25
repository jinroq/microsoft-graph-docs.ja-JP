---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0de6d22d2de42aeb2e00162a35300dea26c1d79e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715875"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/auditLogs/directoryAudits"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *directoryAuditList = [[NSMutableArray alloc] init];
        directoryAuditList = [jsonFinal valueForKey:@"value"];
        MSGraphDirectoryAudit *directoryAudit = [[MSGraphDirectoryAudit alloc] initWithDictionary:[directoryAuditList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```