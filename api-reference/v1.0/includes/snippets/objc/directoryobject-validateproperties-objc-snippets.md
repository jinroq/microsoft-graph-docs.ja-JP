---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e5a30786a72d86ac10833d63ef18f0a030ed2706
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932214"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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