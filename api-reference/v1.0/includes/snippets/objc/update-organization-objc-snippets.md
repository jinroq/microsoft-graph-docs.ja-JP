---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e4055577197c00f87bd96598183101f34afcb75f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738555"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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