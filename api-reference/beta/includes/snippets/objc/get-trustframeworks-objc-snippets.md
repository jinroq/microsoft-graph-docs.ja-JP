---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f50427bef362fc01a793b87c54df4f50573035b2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716757"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/trustFramework/policies"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *trustFrameworkPolicyList = [[NSMutableArray alloc] init];
        trustFrameworkPolicyList = [jsonFinal valueForKey:@"value"];
        MSGraphTrustFrameworkPolicy *trustFrameworkPolicy = [[MSGraphTrustFrameworkPolicy alloc] initWithDictionary:[trustFrameworkPolicyList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```