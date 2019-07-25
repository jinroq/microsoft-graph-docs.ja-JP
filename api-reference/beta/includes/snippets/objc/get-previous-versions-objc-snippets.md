---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4ca2521c618b58063b14795ca0df00a897cc45df
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712857"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{item-id}/versions"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *driveItemVersionList = [[NSMutableArray alloc] init];
        driveItemVersionList = [jsonFinal valueForKey:@"value"];
        MSGraphDriveItemVersion *driveItemVersion = [[MSGraphDriveItemVersion alloc] initWithDictionary:[driveItemVersionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```