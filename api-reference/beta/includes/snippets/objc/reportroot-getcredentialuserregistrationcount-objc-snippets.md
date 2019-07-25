---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f9a6561e34e24a76f96d4da1c4ba7901a6f4bd78
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874114"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getCredentialUserRegistrationCount"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *credentialUserRegistrationCountList = [[NSMutableArray alloc] init];
        credentialUserRegistrationCountList = [jsonFinal valueForKey:@"value"];
        MSGraphCredentialUserRegistrationCount *credentialUserRegistrationCount = [[MSGraphCredentialUserRegistrationCount alloc] initWithDictionary:[credentialUserRegistrationCountList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```