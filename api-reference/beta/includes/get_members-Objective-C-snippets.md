---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2ea0db1a4f8f402361d7e490144b0792fb75e031
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334299"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/11016/members"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *educationUserList = [[NSMutableArray alloc] init];
        educationUserList = [jsonFinal valueForKey:@"value"];
        MSGraphEducationUser *educationUser = [[MSGraphEducationUser alloc] initWithDictionary:[educationUserList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```