---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f964131480f74182f27d715335bd448f7f7c2f9f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35319785"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookTableRow *workbookTableRow = [[MSGraphWorkbookTableRow alloc] init];
MSGraphInt32 *index = [[MSGraphInt32 alloc] init];
[workbookTableRow setIndex:index];

NSError *error;
NSData *workbookTableRowData = [workbookTableRow getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookTableRowData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```