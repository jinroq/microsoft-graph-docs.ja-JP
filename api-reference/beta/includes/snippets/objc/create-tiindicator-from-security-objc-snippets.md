---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3b31ce632404304671f4ac1b6ec4b1e23e5ffe13
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36174749"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/tiIndicators"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTiIndicator *tiIndicator = [[MSGraphTiIndicator alloc] init];
[tiIndicator setAction: [MSGraphTiAction alert]];
NSMutableArray *activityGroupNamesList = [[NSMutableArray alloc] init];
[tiIndicator setActivityGroupNames:activityGroupNamesList];
[tiIndicator setConfidence: 0];
[tiIndicator setDescription:@"This is a canary indicator for demo purpose. Take no action on any observables set in this indicator."];
[tiIndicator setExpirationDateTime: "2019-03-01T21:43:37.5031462+00:00"];
[tiIndicator setExternalId:@"Test--8586509942679764298MS501"];
[tiIndicator setFileHashType: [MSGraphFileHashType sha256]];
[tiIndicator setFileHashValue:@"aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313"];
NSMutableArray *killChainList = [[NSMutableArray alloc] init];
[tiIndicator setKillChain:killChainList];
NSMutableArray *malwareFamilyNamesList = [[NSMutableArray alloc] init];
[tiIndicator setMalwareFamilyNames:malwareFamilyNamesList];
[tiIndicator setSeverity: 0];
NSMutableArray *tagsList = [[NSMutableArray alloc] init];
[tiIndicator setTags:tagsList];
[tiIndicator setTargetProduct:@"Azure Sentinel"];
[tiIndicator setThreatType:@"WatchList"];
[tiIndicator setTlpLevel: [MSGraphTlpLevel green]];

NSError *error;
NSData *tiIndicatorData = [tiIndicator getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tiIndicatorData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```