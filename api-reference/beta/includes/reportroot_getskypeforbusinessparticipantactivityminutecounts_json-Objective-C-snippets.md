---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7aa46d5b64034272ec9f2de8d3e5558f0406c60e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334112"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessParticipantActivityMinuteCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessParticipantActivityMinuteCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessParticipantActivityMinuteCounts *skypeForBusinessParticipantActivityMinuteCounts = [[MSGraphSkypeForBusinessParticipantActivityMinuteCounts alloc] initWithDictionary:[skypeForBusinessParticipantActivityMinuteCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```