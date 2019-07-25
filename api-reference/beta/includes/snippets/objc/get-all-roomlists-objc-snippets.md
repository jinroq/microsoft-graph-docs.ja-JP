---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4b03a83224ddac0e24b9cb85ca1ecc928af09d00
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876789"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/places/microsoft.graph.roomlist"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *roomListList = [[NSMutableArray alloc] init];
        roomListList = [jsonFinal valueForKey:@"value"];
        MSGraphRoomList *roomList = [[MSGraphRoomList alloc] initWithDictionary:[roomListList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```