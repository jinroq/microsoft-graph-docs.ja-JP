---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f6022ee74e6bad922e924fbfaabf30b9f0a09834
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736253"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}/range/format/font"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookRangeFont *workbookRangeFont = [[MSGraphWorkbookRangeFont alloc] init];
[workbookRangeFont setBold: true];
[workbookRangeFont setColor:@"color-value"];
[workbookRangeFont setItalic: true];
[workbookRangeFont setName:@"name-value"];
[workbookRangeFont setSize: 99];
[workbookRangeFont setUnderline:@"underline-value"];

NSError *error;
NSData *workbookRangeFontData = [workbookRangeFont getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookRangeFontData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```