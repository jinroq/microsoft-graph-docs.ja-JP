---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8e69189b0e5485bdbe39f8c24de29f5e3c111b79
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35333723"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookWorksheetList = [[NSMutableArray alloc] init];
        workbookWorksheetList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookWorksheet *workbookWorksheet = [[MSGraphWorkbookWorksheet alloc] initWithDictionary:[workbookWorksheetList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```