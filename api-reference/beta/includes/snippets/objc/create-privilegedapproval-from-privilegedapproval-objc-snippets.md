---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 924b2340a6364f3a3f9150783d416074ec950292
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720313"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedApproval"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrivilegedApproval *privilegedApproval = [[MSGraphPrivilegedApproval alloc] init];
[privilegedApproval setUserId:@"userId-value"];
[privilegedApproval setRoleId:@"roleId-value"];
[privilegedApproval setApprovalType:@"approvalType-value"];
[privilegedApproval setApprovalState: [MSGraphApprovalState pending]];
[privilegedApproval setApprovalDuration:@"datetime-value"];

NSError *error;
NSData *privilegedApprovalData = [privilegedApproval getSerializedDataWithError:&error];
[urlRequest setHTTPBody:privilegedApprovalData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```