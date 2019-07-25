---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a3b102901c34cd4e0902834e1b9d1852eb5fe070
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729126"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOrganization *organization = [[MSGraphOrganization alloc] init];
NSMutableArray *marketingNotificationEmailsList = [[NSMutableArray alloc] init];
[marketingNotificationEmailsList addObject: @"marketing@contoso.com"];
[organization setMarketingNotificationEmails:marketingNotificationEmailsList];
MSGraphPrivacyProfile *privacyProfile = [[MSGraphPrivacyProfile alloc] init];
[privacyProfile setContactEmail:@"alice@contoso.com"];
[privacyProfile setStatementUrl:@"https://contoso.com/privacyStatement"];
[organization setPrivacyProfile:privacyProfile];
NSMutableArray *securityComplianceNotificationMailsList = [[NSMutableArray alloc] init];
[securityComplianceNotificationMailsList addObject: @"security@contoso.com"];
[organization setSecurityComplianceNotificationMails:securityComplianceNotificationMailsList];
NSMutableArray *securityComplianceNotificationPhonesList = [[NSMutableArray alloc] init];
[securityComplianceNotificationPhonesList addObject: @"(123) 456-7890"];
[organization setSecurityComplianceNotificationPhones:securityComplianceNotificationPhonesList];
NSMutableArray *technicalNotificationMailsList = [[NSMutableArray alloc] init];
[technicalNotificationMailsList addObject: @"tech@contoso.com"];
[organization setTechnicalNotificationMails:technicalNotificationMailsList];

NSError *error;
NSData *organizationData = [organization getSerializedDataWithError:&error];
[urlRequest setHTTPBody:organizationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```