---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 48c8f6b2f01c076bb4e913f868407060f5427870
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35325979"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/schemaExtensions/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSchemaExtension *schemaExtension = [[MSGraphSchemaExtension alloc] init];
NSMutableArray *propertiesList = [[NSMutableArray alloc] init];
MSGraphExtensionSchemaProperty *properties = [[MSGraphExtensionSchemaProperty alloc] init];
[properties setName:@"new-name-value"];
[properties setType:@"new-type-value"];
[propertiesList addObject: properties];
MSGraphExtensionSchemaProperty *properties = [[MSGraphExtensionSchemaProperty alloc] init];
[properties setName:@"additional-name-value"];
[properties setType:@"additional-type-value"];
[propertiesList addObject: properties];
[schemaExtension setProperties:propertiesList];

NSError *error;
NSData *schemaExtensionData = [schemaExtension getSerializedDataWithError:&error];
[urlRequest setHTTPBody:schemaExtensionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```