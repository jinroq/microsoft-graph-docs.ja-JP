---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5531abb9b35d859099a3aa7c090fc63a3696bde4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35325927"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/users/{user-id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationUser *educationUser = [[MSGraphEducationUser alloc] init];
[educationUser setDisplayName:@"Rogelio Cazares"];
[educationUser setGivenName:@"Rogelio"];
[educationUser setMiddleName:@"Fernando"];
[educationUser setSurname:@"Cazares"];

NSError *error;
NSData *educationUserData = [educationUser getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationUserData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```