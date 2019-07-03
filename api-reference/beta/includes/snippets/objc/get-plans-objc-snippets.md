---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a7353acfe2c35ce3135fbd6741412ec054f90f1f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503845"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/planner/plans"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *plannerPlanList = [[NSMutableArray alloc] init];
        plannerPlanList = [jsonFinal valueForKey:@"value"];
        MSGraphPlannerPlan *plannerPlan = [[MSGraphPlannerPlan alloc] initWithDictionary:[plannerPlanList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```