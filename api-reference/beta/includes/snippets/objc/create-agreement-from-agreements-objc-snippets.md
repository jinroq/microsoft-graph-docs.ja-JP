---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 412cddf5caf8ee8c1290d54cec6363e62599c02d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710528"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/agreements"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAgreement *agreement = [[MSGraphAgreement alloc] init];
[agreement setDisplayName:@"MSGraph Sample"];
[agreement setIsViewingBeforeAcceptanceRequired: true];
NSMutableArray *filesList = [[NSMutableArray alloc] init];
MSGraphAgreementFile *files = [[MSGraphAgreementFile alloc] init];
[files setFileName:@"TOU.pdf"];
[files setLanguage:@"en"];
[files setIsDefault: true];
MSGraphAgreementFileData *fileData = [[MSGraphAgreementFileData alloc] init];
[fileData setData:@"SGVsbG8gd29ybGQ="];
[files setFileData:fileData];
[filesList addObject: files];
[agreement setFiles:filesList];

NSError *error;
NSData *agreementData = [agreement getSerializedDataWithError:&error];
[urlRequest setHTTPBody:agreementData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```