---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 55d61b9b8b3efd33d070779ffd127dd7a948a96e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35325748"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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