---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4e7c5367257e0c66cf971fa7580013ba80077d74
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334610"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/timeOffReasons"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *timeOffReasonList = [[NSMutableArray alloc] init];
        timeOffReasonList = [jsonFinal valueForKey:@"value"];
        MSGraphTimeOffReason *timeOffReason = [[MSGraphTimeOffReason alloc] initWithDictionary:[timeOffReasonList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```