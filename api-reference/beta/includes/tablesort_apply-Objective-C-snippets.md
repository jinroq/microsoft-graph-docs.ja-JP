---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ef512b48ab1dbea491969118e0dcff8bb9c200ff
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334651"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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