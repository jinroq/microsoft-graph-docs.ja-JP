---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2d39b56d48a060fbccf5502eda641a2ce2ad1012
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35315035"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/buckets/{id}"]]];
[urlRequest setHTTPMethod:@"DELETE"];
[urlRequest setValue:@"W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"" forHTTPHeaderField:@"If-Match"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```