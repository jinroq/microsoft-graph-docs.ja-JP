---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 16f122a44bff5cd0fe4345997fecb732b82d47c6
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933957"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/app/calls/{id}/audioRoutingGroups/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAudioRoutingGroup *audioRoutingGroup = [[MSGraphAudioRoutingGroup alloc] init];
[audioRoutingGroup setId:@"oneToOne"];
[audioRoutingGroup setRoutingMode: [MSGraphRoutingMode oneToOne]];
NSMutableArray *sourcesList = [[NSMutableArray alloc] init];
[sourcesList addObject: @"632899f8-2ea1-4604-8413-27bd2892079f"];
[audioRoutingGroup setSources:sourcesList];
NSMutableArray *receiversList = [[NSMutableArray alloc] init];
[receiversList addObject: @"550fae72-d251-43ec-868c-373732c2704f"];
[receiversList addObject: @"72f988bf-86f1-41af-91ab-2d7cd011db47"];
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