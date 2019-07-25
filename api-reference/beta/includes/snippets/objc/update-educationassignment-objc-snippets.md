---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 143c4e81530e18f81d08f2cb7c0b06ffcc53317d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712878"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/11021/assignments/19002"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationAssignment *educationAssignment = [[MSGraphEducationAssignment alloc] init];
[educationAssignment setDisplayName:@"Week 1 reading assignment"];
MSGraphEducationItemBody *instructions = [[MSGraphEducationItemBody alloc] init];
[instructions setContentType: [MSGraphBodyType text]];
[instructions setContent:@"Read chapters 1 through 3"];
[educationAssignment setInstructions:instructions];
[educationAssignment setDueDateTime: "2014-02-01T00:00:00Z"];

NSError *error;
NSData *educationAssignmentData = [educationAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```