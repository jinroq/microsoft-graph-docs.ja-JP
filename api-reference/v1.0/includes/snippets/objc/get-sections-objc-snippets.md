---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a286c7fa0c851c4c6b76163a2d47357e9fe630ca
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895093"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onenote/sectionGroups/{id}/sections"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *onenoteSectionList = [[NSMutableArray alloc] init];
        onenoteSectionList = [jsonFinal valueForKey:@"value"];
        MSGraphOnenoteSection *onenoteSection = [[MSGraphOnenoteSection alloc] initWithDictionary:[onenoteSectionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```