---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 826b296782ce8504cd7251570995abe2a2aa7829
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720711"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{id|userPrincipalName}/photo"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphProfilePhoto *profilePhoto = [[MSGraphProfilePhoto alloc] init];
[profilePhoto setHeight: 99];
[profilePhoto setWidth: 99];
[profilePhoto setId:@"id-value"];

NSError *error;
NSData *profilePhotoData = [profilePhoto getSerializedDataWithError:&error];
[urlRequest setHTTPBody:profilePhotoData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```