---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8bbccbdee40ea588e7f7d0c6de85778f93478078
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334619"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill"]]];
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