---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 64e33fb663c74c5e3c61bc80a66983d300ac8987
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35326217"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/me/schools"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *educationSchoolList = [[NSMutableArray alloc] init];
        educationSchoolList = [jsonFinal valueForKey:@"value"];
        MSGraphEducationSchool *educationSchool = [[MSGraphEducationSchool alloc] initWithDictionary:[educationSchoolList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```