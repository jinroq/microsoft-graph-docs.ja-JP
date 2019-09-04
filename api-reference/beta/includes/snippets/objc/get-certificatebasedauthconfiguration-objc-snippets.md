---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 33e4da6805dfdd2c4ca8f9d02239c4d78d613be7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720117"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/{id}/certificateBasedAuthConfiguration/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphCertificateBasedAuthConfiguration *certificateBasedAuthConfiguration = [[MSGraphCertificateBasedAuthConfiguration alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```