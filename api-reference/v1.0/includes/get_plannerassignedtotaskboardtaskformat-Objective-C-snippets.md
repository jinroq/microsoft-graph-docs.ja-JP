---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b4a14a02d551f20e8387c8c1895eb124a45967cc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35325873"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/tasks/{task-id}/assignedToTaskBoardFormat"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPlannerAssignedToTaskBoardTaskFormat *plannerAssignedToTaskBoardTaskFormat = [[MSGraphPlannerAssignedToTaskBoardTaskFormat alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```