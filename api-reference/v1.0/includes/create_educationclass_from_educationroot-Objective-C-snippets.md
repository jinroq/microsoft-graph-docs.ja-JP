---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e4aad042316b00ae58fd78c6dfff9a53823e9301
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35317255"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationClass *educationClass = [[MSGraphEducationClass alloc] init];
[educationClass setDescription:@"Health Level 1"];
[educationClass setClassCode:@"Health 501"];
[educationClass setDisplayName:@"Health 1"];
[educationClass setExternalId:@"11019"];
[educationClass setExternalName:@"Health Level 1"];
[educationClass setExternalSource: [MSGraphEducationExternalSource sis]];
[educationClass setMailNickname:@"fineartschool.net"];

NSError *error;
NSData *educationClassData = [educationClass getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationClassData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```