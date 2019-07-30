---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5b889c18d229e22625743483b2ce0a780e587b0a
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933984"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/app/calls/{id}/audioRoutingGroups"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAudioRoutingGroup *audioRoutingGroup = [[MSGraphAudioRoutingGroup alloc] init];
[audioRoutingGroup setId:@"oneToOne"];
[audioRoutingGroup setRoutingMode: [MSGraphRoutingMode oneToOne]];
NSMutableArray *sourcesList = [[NSMutableArray alloc] init];
[sourcesList addObject: @"632899f8-2ea1-4604-8413-27bd2892079f"];
[audioRoutingGroup setSources:sourcesList];
NSMutableArray *receiversList = [[NSMutableArray alloc] init];
[receiversList addObject: @"550fae72-d251-43ec-868c-373732c2704f"];
[audioRoutingGroup setReceivers:receiversList];

NSError *error;
NSData *audioRoutingGroupData = [audioRoutingGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:audioRoutingGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```