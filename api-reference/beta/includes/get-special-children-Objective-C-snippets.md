---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6a8b87302e5113a6e302779aa70a092ddb162974
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35333637"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/special/{name}/children"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *driveItemList = [[NSMutableArray alloc] init];
        driveItemList = [jsonFinal valueForKey:@"value"];
        MSGraphDriveItem *driveItem = [[MSGraphDriveItem alloc] initWithDictionary:[driveItemList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```