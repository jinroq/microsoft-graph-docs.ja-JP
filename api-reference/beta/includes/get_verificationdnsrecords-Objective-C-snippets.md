---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d741f9e24f7fbcca40721f58ff8d0ff75f0251ad
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35316070"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/domains/contoso.com/verificationDnsRecords"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *domainDnsRecordList = [[NSMutableArray alloc] init];
        domainDnsRecordList = [jsonFinal valueForKey:@"value"];
        MSGraphDomainDnsRecord *domainDnsRecord = [[MSGraphDomainDnsRecord alloc] initWithDictionary:[domainDnsRecordList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```