---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b9b00252feeecb975fba4b6fa0f563c1c4f2c23b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739831"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *fieldsList = [[NSMutableArray alloc] init];
MSGraphWorkbookSortField *fields = [[MSGraphWorkbookSortField alloc] init];
[fields setKey: 99];
[fields setSortOn:@"sortOn-value"];
[fields setAscending: true];
[fields setColor:@"color-value"];
[fields setDataOption:@"dataOption-value"];
MSGraphWorkbookIcon *icon = [[MSGraphWorkbookIcon alloc] init];
[icon setSet:@"set-value"];
[icon setIndex: 99];
[fields setIcon:icon];
[fieldsList addObject: fields];
payloadDictionary[@"fields"] = fieldsList;

BOOL matchCase = YES;
payloadDictionary[@"matchCase"] = matchCase;

NSString *method = @"method-value";
payloadDictionary[@"method"] = method;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```