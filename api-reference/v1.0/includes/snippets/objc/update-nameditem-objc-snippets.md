---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5bbd589495cc05953a6fb2486d6aae42e059d5ac
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738822"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookNamedItem *workbookNamedItem = [[MSGraphWorkbookNamedItem alloc] init];
[workbookNamedItem setType:@"type-value"];
[workbookNamedItem setScope:@"scope-value"];
[workbookNamedItem setComment:@"comment-value"];
MSGraphJson *value = [[MSGraphJson alloc] init];
[workbookNamedItem setValue:value];
[workbookNamedItem setVisible: true];

NSError *error;
NSData *workbookNamedItemData = [workbookNamedItem getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookNamedItemData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```