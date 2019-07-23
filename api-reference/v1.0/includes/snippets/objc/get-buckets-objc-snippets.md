---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 54642202fa7d87cca46ecc965d665093208b24b1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733277"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/plans/{plan-id}/buckets"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *plannerBucketList = [[NSMutableArray alloc] init];
        plannerBucketList = [jsonFinal valueForKey:@"value"];
        MSGraphPlannerBucket *plannerBucket = [[MSGraphPlannerBucket alloc] initWithDictionary:[plannerBucketList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```