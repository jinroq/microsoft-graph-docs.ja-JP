---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6def9adb30f97d6c19655d2b82b3f53e29597fb1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723225"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/messages"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMessage *message = [[MSGraphMessage alloc] init];
[message setSubject:@"9/8/2018: concert"];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"The group represents Washington."];
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
[internetMessageHeaders setValue:@"Washington"];
[internetMessageHeadersList addObject: internetMessageHeaders];
MSGraphInternetMessageHeader *internetMessageHeaders = [[MSGraphInternetMessageHeader alloc] init];
[internetMessageHeaders setName:@"x-custom-header-group-id"];
[internetMessageHeaders setValue:@"WA001"];
[internetMessageHeadersList addObject: internetMessageHeaders];
[message setInternetMessageHeaders:internetMessageHeadersList];

NSError *error;
NSData *messageData = [message getSerializedDataWithError:&error];
[urlRequest setHTTPBody:messageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```