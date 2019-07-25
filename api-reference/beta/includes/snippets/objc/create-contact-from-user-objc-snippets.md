---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0384db6ec08f642f945e36fa4500f486effc0db2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716405"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contacts"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContact *contact = [[MSGraphContact alloc] init];
[contact setGivenName:@"Pavel"];
[contact setSurname:@"Bansky"];
NSMutableArray *emailAddressesList = [[NSMutableArray alloc] init];
MSGraphTypedEmailAddress *emailAddresses = [[MSGraphTypedEmailAddress alloc] init];
[emailAddresses setAddress:@"pavelb@contoso.onmicrosoft.com"];
[emailAddresses setName:@"Pavel Bansky"];
[emailAddresses setType: [MSGraphEmailType personal]];
[emailAddressesList addObject: emailAddresses];
MSGraphTypedEmailAddress *emailAddresses = [[MSGraphTypedEmailAddress alloc] init];
[emailAddresses setAddress:@"pavelb@fabrikam.onmicrosoft.com"];
[emailAddresses setName:@"Pavel Bansky"];
[emailAddresses setType: [MSGraphEmailType other]];
[emailAddresses setOtherLabel:@"Volunteer work"];
[emailAddressesList addObject: emailAddresses];
[contact setEmailAddresses:emailAddressesList];
NSMutableArray *phonesList = [[NSMutableArray alloc] init];
MSGraphPhone *phones = [[MSGraphPhone alloc] init];
[phones setNumber:@"+1 732 555 0102"];
[phones setType: [MSGraphPhoneType business]];
[phonesList addObject: phones];
[contact setPhones:phonesList];

NSError *error;
NSData *contactData = [contact getSerializedDataWithError:&error];
[urlRequest setHTTPBody:contactData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```