---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7f87d1fd995e3d6856409489ec8b1ca456f6fe0b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35325420"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/{class-id}/teachers"]]];
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