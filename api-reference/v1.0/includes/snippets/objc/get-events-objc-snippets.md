---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 595a85ef6a2e8997014380f0ef2556eb77cf96e5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714551"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"outlook.timezone=\"Pacific Standard Time\"" forHTTPHeaderField:@"Prefer"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *eventList = [[NSMutableArray alloc] init];
        eventList = [jsonFinal valueForKey:@"value"];
        MSGraphEvent *event = [[MSGraphEvent alloc] initWithDictionary:[eventList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```