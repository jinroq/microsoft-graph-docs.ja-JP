---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9fed70fb403838c3fd46e567dae5bfc95fe6d479
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712962"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{item-id}/invite"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *recipientsList = [[NSMutableArray alloc] init];
MSGraphDriveRecipient *recipients = [[MSGraphDriveRecipient alloc] init];
[recipients setEmail:@"ryan@contoso.org"];
[recipientsList addObject: recipients];
payloadDictionary[@"recipients"] = recipientsList;

NSString *message = @"Here's the file that we're collaborating on.";
payloadDictionary[@"message"] = message;

BOOL requireSignIn = YES;
payloadDictionary[@"requireSignIn"] = requireSignIn;

BOOL sendInvitation = YES;
payloadDictionary[@"sendInvitation"] = sendInvitation;

NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"write"];
payloadDictionary[@"roles"] = rolesList;

NSString *password = @"password123";
payloadDictionary[@"password"] = password;

NSString *expirationDateTimeDateTimeString = @"07/15/2018 14:00:00";
NSDate *expirationDateTime = [NSDate ms_dateFromString: expirationDateTimeDateTimeString];
payloadDictionary[@"expirationDateTime"] = expirationDateTime;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```