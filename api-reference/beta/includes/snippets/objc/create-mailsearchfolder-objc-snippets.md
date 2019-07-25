---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bbb798c0a7a1447e5a69625ff06f7cc63f99c7c9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721573"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMailFolder *mailFolder = [[MSGraphMailFolder alloc] init];
[mailFolder setDisplayName:@"Weekly digests"];
[mailFolder setIncludeNestedFolders: true];
NSMutableArray *sourceFolderIdsList = [[NSMutableArray alloc] init];
[sourceFolderIdsList addObject: @"AQMkADYAAAIBDAAAAA=="];
[mailFolder setSourceFolderIds:sourceFolderIdsList];
[mailFolder setFilterQuery:@"contains(subject, 'weekly digest')"];

NSError *error;
NSData *mailFolderData = [mailFolder getSerializedDataWithError:&error];
[urlRequest setHTTPBody:mailFolderData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```