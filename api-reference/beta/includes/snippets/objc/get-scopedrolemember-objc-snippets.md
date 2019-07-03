---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f7360a733d11096d295f4f504dcd5eeebbc99cdd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485963"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/administrativeUnits/{id}/scopedRoleMembers"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *scopedRoleMembershipList = [[NSMutableArray alloc] init];
        scopedRoleMembershipList = [jsonFinal valueForKey:@"value"];
        MSGraphScopedRoleMembership *scopedRoleMembership = [[MSGraphScopedRoleMembership alloc] initWithDictionary:[scopedRoleMembershipList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```