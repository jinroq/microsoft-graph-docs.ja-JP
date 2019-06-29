---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b032a8a6052857eb4f6d8f1bd29189137604790e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35325672"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directoryRoleTemplates"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *directoryRoleTemplateList = [[NSMutableArray alloc] init];
        directoryRoleTemplateList = [jsonFinal valueForKey:@"value"];
        MSGraphDirectoryRoleTemplate *directoryRoleTemplate = [[MSGraphDirectoryRoleTemplate alloc] initWithDictionary:[directoryRoleTemplateList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```