---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d0b572d04ff794ce963cd4864d132e5ca687c1c2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471519"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/fill"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookRangeFill *workbookRangeFill = [[MSGraphWorkbookRangeFill alloc] init];
[workbookRangeFill setColor:@"#0000FF"];

NSError *error;
NSData *workbookRangeFillData = [workbookRangeFill getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookRangeFillData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```