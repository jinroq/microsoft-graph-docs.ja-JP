---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 152252271876de41a80b210ae56e679414d2028a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35319976"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/invitations"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphInvitation *invitation = [[MSGraphInvitation alloc] init];
[invitation setInvitedUserEmailAddress:@"yyy@test.com"];
[invitation setInviteRedirectUrl:@"https://myapp.com"];

NSError *error;
NSData *invitationData = [invitation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:invitationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```