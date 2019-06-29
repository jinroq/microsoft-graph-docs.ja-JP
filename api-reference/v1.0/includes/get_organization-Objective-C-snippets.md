---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bb17b952ea4196073d6cf219dd7c9fa210e26051
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35325669"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *organizationList = [[NSMutableArray alloc] init];
        organizationList = [jsonFinal valueForKey:@"value"];
        MSGraphOrganization *organization = [[MSGraphOrganization alloc] initWithDictionary:[organizationList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```