---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e501ee63de61750550e8950ff850bf5eb372de28
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740293"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphWorkbookFilterCriteria *criteria = [[MSGraphWorkbookFilterCriteria alloc] init];
[criteria setCriterion1:@"criterion1-value"];
[criteria setCriterion2:@"criterion2-value"];
[criteria setColor:@"color-value"];
MSGraphString *operator = [[MSGraphString alloc] init];
[criteria setOperator:operator];
MSGraphWorkbookIcon *icon = [[MSGraphWorkbookIcon alloc] init];
[icon setSet:@"set-value"];
[icon setIndex: 99];
[criteria setIcon:icon];
[criteria setDynamicCriteria:@"dynamicCriteria-value"];
MSGraphJson *values = [[MSGraphJson alloc] init];
[criteria setValues:values];
[criteria setFilterOn:@"filterOn-value"];
payloadDictionary[@"criteria"] = criteria;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```