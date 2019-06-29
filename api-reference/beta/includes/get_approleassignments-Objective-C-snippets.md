---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 259a86a0a8f6f89a9f2f3dee0dc02efc01fbc8d3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35316104"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/appRoleAssignments"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *appRoleAssignmentList = [[NSMutableArray alloc] init];
        appRoleAssignmentList = [jsonFinal valueForKey:@"value"];
        MSGraphAppRoleAssignment *appRoleAssignment = [[MSGraphAppRoleAssignment alloc] initWithDictionary:[appRoleAssignmentList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```