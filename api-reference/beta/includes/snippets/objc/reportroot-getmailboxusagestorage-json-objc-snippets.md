---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 84098f5817194afaba670532e986b3db1b90fe83
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727530"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getMailboxUsageStorage(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *mailboxUsageStorageList = [[NSMutableArray alloc] init];
        mailboxUsageStorageList = [jsonFinal valueForKey:@"value"];
        MSGraphMailboxUsageStorage *mailboxUsageStorage = [[MSGraphMailboxUsageStorage alloc] initWithDictionary:[mailboxUsageStorageList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```