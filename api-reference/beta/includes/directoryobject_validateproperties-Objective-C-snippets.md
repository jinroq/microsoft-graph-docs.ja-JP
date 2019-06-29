---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35d8d34e357b60a43a53795a6042a1853c2c5375
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35333993"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directoryObjects/validateProperties"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *entityType = @"Group";
payloadDictionary[@"entityType"] = entityType;

NSString *displayName = @"Myprefix_test_mysuffix";
payloadDictionary[@"displayName"] = displayName;

NSString *mailNickname = @"Myprefix_test_mysuffix";
payloadDictionary[@"mailNickname"] = mailNickname;

NSString *onBehalfOfUserId = @"onBehalfOfUserId-value";
payloadDictionary[@"onBehalfOfUserId"] = onBehalfOfUserId;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```