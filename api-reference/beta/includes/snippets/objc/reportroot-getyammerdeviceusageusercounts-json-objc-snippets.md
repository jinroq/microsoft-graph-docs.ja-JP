---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6b7e175c3baab7a8c1b5b3df09cf4e38e409ebe3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726351"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *yammerDeviceUsageUserCountsList = [[NSMutableArray alloc] init];
        yammerDeviceUsageUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphYammerDeviceUsageUserCounts *yammerDeviceUsageUserCounts = [[MSGraphYammerDeviceUsageUserCounts alloc] initWithDictionary:[yammerDeviceUsageUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```