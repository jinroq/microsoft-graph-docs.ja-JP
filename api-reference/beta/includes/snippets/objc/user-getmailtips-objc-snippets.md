---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a6e12741b3620cf6f1af14c6ffad66be34e673a9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716610"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/getMailTips"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *emailAddressesList = [[NSMutableArray alloc] init];
[emailAddressesList addObject: @"danas@contoso.onmicrosoft.com"];
[emailAddressesList addObject: @"fannyd@contoso.onmicrosoft.com"];
payloadDictionary[@"EmailAddresses"] = emailAddressesList;

MSGraphMailTipsType *mailTipsOptions = [MSGraphMailTipsType automaticReplies];
payloadDictionary[@"MailTipsOptions"] = mailTipsOptions;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```