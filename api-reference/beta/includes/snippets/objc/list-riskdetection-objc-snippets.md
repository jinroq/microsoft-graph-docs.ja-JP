---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9bcc85988596524428a11a681b35e54afeb9500a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725772"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/riskDetections"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *riskDetectionList = [[NSMutableArray alloc] init];
        riskDetectionList = [jsonFinal valueForKey:@"value"];
        MSGraphRiskDetection *riskDetection = [[MSGraphRiskDetection alloc] initWithDictionary:[riskDetectionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```