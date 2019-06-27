---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0b781da3d78ed31326233335517573ce71587b91
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334301"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/masterCategories"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *outlookCategoryList = [[NSMutableArray alloc] init];
        outlookCategoryList = [jsonFinal valueForKey:@"value"];
        MSGraphOutlookCategory *outlookCategory = [[MSGraphOutlookCategory alloc] initWithDictionary:[outlookCategoryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```