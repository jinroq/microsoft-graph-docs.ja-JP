---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d9ae5d1d3247db3dc1a574d9dc77636980dcb2ca
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486614"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/schedulingGroups"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSchedulingGroup *schedulingGroup = [[MSGraphSchedulingGroup alloc] init];
[schedulingGroup setDisplayName:@"Cashiers"];
[schedulingGroup setIsActive: true];
NSMutableArray *userIdsList = [[NSMutableArray alloc] init];
[userIdsList addObject: @"c5d0c76b-80c4-481c-be50-923cd8d680a1"];
[userIdsList addObject: @"2a4296b3-a28a-44ba-bc66-0274b9b95851"];
[schedulingGroup setUserIds:userIdsList];

NSError *error;
NSData *schedulingGroupData = [schedulingGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:schedulingGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```