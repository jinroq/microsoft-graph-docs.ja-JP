---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: eaf47fd5d6c61b4b85e31b74fab7b957fe8d9f4a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35325552"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOutlookCategory *outlookCategory = [[MSGraphOutlookCategory alloc] init];
[outlookCategory setColor: [MSGraphCategoryColor preset15]];

NSError *error;
NSData *outlookCategoryData = [outlookCategory getSerializedDataWithError:&error];
[urlRequest setHTTPBody:outlookCategoryData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```