---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca2b5456dbaa0f8dbb6384e5b5c89da05be977bc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711413"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/sendMail"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphMessage *message = [[MSGraphMessage alloc] init];
[message setSubject:@"9/9/2018: concert"];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"The group represents Nevada."];
[message setBody:body];
NSMutableArray *toRecipientsList = [[NSMutableArray alloc] init];
MSGraphRecipient *toRecipients = [[MSGraphRecipient alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setAddress:@"AlexW@contoso.OnMicrosoft.com"];
[toRecipients setEmailAddress:emailAddress];
[toRecipientsList addObject: toRecipients];
[message setToRecipients:toRecipientsList];
NSMutableArray *internetMessageHeadersList = [[NSMutableArray alloc] init];
MSGraphInternetMessageHeader *internetMessageHeaders = [[MSGraphInternetMessageHeader alloc] init];
[internetMessageHeaders setName:@"x-custom-header-group-name"];
[internetMessageHeaders setValue:@"Nevada"];
[internetMessageHeadersList addObject: internetMessageHeaders];
MSGraphInternetMessageHeader *internetMessageHeaders = [[MSGraphInternetMessageHeader alloc] init];
[internetMessageHeaders setName:@"x-custom-header-group-id"];
[internetMessageHeaders setValue:@"NV001"];
[internetMessageHeadersList addObject: internetMessageHeaders];
[message setInternetMessageHeaders:internetMessageHeadersList];
payloadDictionary[@"message"] = message;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```