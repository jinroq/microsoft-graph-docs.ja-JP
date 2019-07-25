---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 608518423bde7dce6f9526210187420990289f39
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716667"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/findRooms"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAddressList = [[NSMutableArray alloc] init];
        emailAddressList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] initWithDictionary:[emailAddressList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```