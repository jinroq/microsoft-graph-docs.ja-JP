---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f349fa468ae3235674f86c23d52286c6df269c49
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35314945"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailFolders/inbox/messageRules"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *messageRuleList = [[NSMutableArray alloc] init];
        messageRuleList = [jsonFinal valueForKey:@"value"];
        MSGraphMessageRule *messageRule = [[MSGraphMessageRule alloc] initWithDictionary:[messageRuleList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```