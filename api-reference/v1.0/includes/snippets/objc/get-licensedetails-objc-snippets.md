---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 407190cac82272ed7fd6d3f298f38c7b0da70e37
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731198"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/licenseDetails"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *licenseDetailsList = [[NSMutableArray alloc] init];
        licenseDetailsList = [jsonFinal valueForKey:@"value"];
        MSGraphLicenseDetails *licenseDetails = [[MSGraphLicenseDetails alloc] initWithDictionary:[licenseDetailsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```