---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 227b732f71b797975dc027a2e5bb8876cd028a86
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172970"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/featureRolloutPolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphFeatureRolloutPolicy *featureRolloutPolicy = [[MSGraphFeatureRolloutPolicy alloc] init];
[featureRolloutPolicy setDisplayName:@"PassthroughAuthentication rollout policy"];
[featureRolloutPolicy setDescription:@"PassthroughAuthentication rollout policy"];
[featureRolloutPolicy setFeature: [MSGraphStagedFeatureName passthroughAuthentication]];
[featureRolloutPolicy setIsEnabled: true];
[featureRolloutPolicy setIsAppliedToOrganization: false];

NSError *error;
NSData *featureRolloutPolicyData = [featureRolloutPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:featureRolloutPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```