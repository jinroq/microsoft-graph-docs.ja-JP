---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f93525ed2c2c880c744b63a07c56a94622542ba9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526319"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}/range/sort/apply"]]];
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

BOOL hasHeaders = YES;
payloadDictionary[@"hasHeaders"] = hasHeaders;

NSString *orientation = @"orientation-value";
payloadDictionary[@"orientation"] = orientation;

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