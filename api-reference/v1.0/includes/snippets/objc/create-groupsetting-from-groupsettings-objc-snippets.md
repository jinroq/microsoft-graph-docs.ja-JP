---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bdd8b21fbd4c9e937aadfff3ee8bf670c534a595
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741224"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groupSettings"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGroupSetting *groupSetting = [[MSGraphGroupSetting alloc] init];
[groupSetting setDisplayName:@"displayName-value"];
[groupSetting setTemplateId:@"templateId-value"];
NSMutableArray *valuesList = [[NSMutableArray alloc] init];
MSGraphSettingValue *values = [[MSGraphSettingValue alloc] init];
[values setName:@"name-value"];
[values setValue:@"value-value"];
[valuesList addObject: values];
[groupSetting setValues:valuesList];

NSError *error;
NSData *groupSettingData = [groupSetting getSerializedDataWithError:&error];
[urlRequest setHTTPBody:groupSettingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```