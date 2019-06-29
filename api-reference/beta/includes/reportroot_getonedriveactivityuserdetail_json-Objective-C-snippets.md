---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7d5b8a42de9eeb7e16ef3428580af3f764f2624d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334585"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *oneDriveActivityUserDetailList = [[NSMutableArray alloc] init];
        oneDriveActivityUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphOneDriveActivityUserDetail *oneDriveActivityUserDetail = [[MSGraphOneDriveActivityUserDetail alloc] initWithDictionary:[oneDriveActivityUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```