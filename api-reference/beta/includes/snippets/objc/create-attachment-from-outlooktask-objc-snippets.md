---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9dffedcf3ddbc957bc95a0a7ae168e883d820e6b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728979"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{id}/outlook/tasks/{id}/attachments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAttachment *attachment = [[MSGraphAttachment alloc] init];
[attachment setLastModifiedDateTime:@"datetime-value"];
[attachment setName:@"name-value"];
[attachment setContentType:@"contentType-value"];
[attachment setSize: 99];
[attachment setIsInline: true];

NSError *error;
NSData *attachmentData = [attachment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:attachmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```