---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 84279528cf6e5c97525c86a81458bef4a7de39c4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334075"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *riskyUserHistoryItemList = [[NSMutableArray alloc] init];
        riskyUserHistoryItemList = [jsonFinal valueForKey:@"value"];
        MSGraphRiskyUserHistoryItem *riskyUserHistoryItem = [[MSGraphRiskyUserHistoryItem alloc] initWithDictionary:[riskyUserHistoryItemList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```