---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5317375568413ae88d1186e70a2abc80524874a5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35326013"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/messages"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMessage *message = [[MSGraphMessage alloc] init];
[message setSubject:@"Did you see last night's game?"];
[message setImportance: [MSGraphImportance low]];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"They were <b>awesome</b>!"];
[message setBody:body];
NSMutableArray *toRecipientsList = [[NSMutableArray alloc] init];
MSGraphRecipient *toRecipients = [[MSGraphRecipient alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setAddress:@"AdeleV@contoso.onmicrosoft.com"];
[toRecipients setEmailAddress:emailAddress];
[toRecipientsList addObject: toRecipients];
[message setToRecipients:toRecipientsList];

NSError *error;
NSData *messageData = [message getSerializedDataWithError:&error];
[urlRequest setHTTPBody:messageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```