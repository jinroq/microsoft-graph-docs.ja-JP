---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7803b37f73a5f0ecc764e70cfc5417f55618b5fc
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460995"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/me/assignments/{id}/submissions/{id}/outcomes"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *educationOutcomeList = [[NSMutableArray alloc] init];
        educationOutcomeList = [jsonFinal valueForKey:@"value"];
        MSGraphEducationOutcome *educationOutcome = [[MSGraphEducationOutcome alloc] initWithDictionary:[educationOutcomeList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```