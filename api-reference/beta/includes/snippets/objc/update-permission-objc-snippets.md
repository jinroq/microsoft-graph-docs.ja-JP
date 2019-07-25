---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 677a2746a59029dd61fa6b33a5e4107c77ea7527
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730542"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{item-id}/permissions/{perm-id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPermission *permission = [[MSGraphPermission alloc] init];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"read"];
[permission setRoles:rolesList];

NSError *error;
NSData *permissionData = [permission getSerializedDataWithError:&error];
[urlRequest setHTTPBody:permissionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```