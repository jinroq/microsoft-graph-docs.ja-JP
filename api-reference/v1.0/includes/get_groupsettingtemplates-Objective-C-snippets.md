---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 47c2ffc252d32109e5d15f619a944a920d43598a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35325334"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groupSettingTemplates"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *groupSettingTemplateList = [[NSMutableArray alloc] init];
        groupSettingTemplateList = [jsonFinal valueForKey:@"value"];
        MSGraphGroupSettingTemplate *groupSettingTemplate = [[MSGraphGroupSettingTemplate alloc] initWithDictionary:[groupSettingTemplateList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```