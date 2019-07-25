---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9e00f996d68618f55690418f328771e84ab30335
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720145"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedRoleAssignmentRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrivilegedRoleAssignmentRequest *privilegedRoleAssignmentRequest = [[MSGraphPrivilegedRoleAssignmentRequest alloc] init];
[privilegedRoleAssignmentRequest setDuration:@"2"];
[privilegedRoleAssignmentRequest setReason:@"Activate the role for business purpose"];
[privilegedRoleAssignmentRequest setTicketNumber:@"234"];
[privilegedRoleAssignmentRequest setTicketSystem:@"system"];
MSGraphGovernanceSchedule *schedule = [[MSGraphGovernanceSchedule alloc] init];
[schedule setStartDateTime: "2018-02-08T02:35:17.903Z"];
[privilegedRoleAssignmentRequest setSchedule:schedule];
[privilegedRoleAssignmentRequest setEvaluateOnly: false];
[privilegedRoleAssignmentRequest setType:@"UserAdd"];
[privilegedRoleAssignmentRequest setAssignmentState:@"Active"];
[privilegedRoleAssignmentRequest setRoleId:@"88d8e3e3-8f55-4a1e-953a-9b9898b8876b"];

NSError *error;
NSData *privilegedRoleAssignmentRequestData = [privilegedRoleAssignmentRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:privilegedRoleAssignmentRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```