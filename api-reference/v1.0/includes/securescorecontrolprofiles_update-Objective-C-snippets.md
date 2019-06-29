---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a57b187d01e932c26767d0bd0a54ec38565a5df5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35317236"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/secureScoreControlProfiles/NonOwnerAccess"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSecureScoreControlProfile *secureScoreControlProfile = [[MSGraphSecureScoreControlProfile alloc] init];
[secureScoreControlProfile setAssignedTo:@""];
[secureScoreControlProfile setComment:@"control is reviewed"];
[secureScoreControlProfile setState:@"Reviewed"];
MSGraphSecurityVendorInformation *vendorInformation = [[MSGraphSecurityVendorInformation alloc] init];
[vendorInformation setProvider:@"SecureScore"];
[vendorInformation setProviderVersion: null];
[vendorInformation setSubProvider: null];
[vendorInformation setVendor:@"Microsoft"];
[secureScoreControlProfile setVendorInformation:vendorInformation];

NSError *error;
NSData *secureScoreControlProfileData = [secureScoreControlProfile getSerializedDataWithError:&error];
[urlRequest setHTTPBody:secureScoreControlProfileData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```