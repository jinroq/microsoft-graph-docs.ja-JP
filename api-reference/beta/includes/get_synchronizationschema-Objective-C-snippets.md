---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 315c664def343a8758292b07070131c281977caf
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334155"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"Bearer {Token}" forHTTPHeaderField:@"Authorization"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphSynchronizationSchema *synchronizationSchema = [[MSGraphSynchronizationSchema alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```