---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca366150fe43e2100993d0e69764f3a11e23f64d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35316116"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *timeZoneInformationList = [[NSMutableArray alloc] init];
        timeZoneInformationList = [jsonFinal valueForKey:@"value"];
        MSGraphTimeZoneInformation *timeZoneInformation = [[MSGraphTimeZoneInformation alloc] initWithDictionary:[timeZoneInformationList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```