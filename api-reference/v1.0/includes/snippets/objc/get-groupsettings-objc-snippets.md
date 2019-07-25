---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f5a8caf5ef5b0f16e151583008d7acc68f379a03
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722452"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groupSettings"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *groupSettingList = [[NSMutableArray alloc] init];
        groupSettingList = [jsonFinal valueForKey:@"value"];
        MSGraphGroupSetting *groupSetting = [[MSGraphGroupSetting alloc] initWithDictionary:[groupSettingList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```