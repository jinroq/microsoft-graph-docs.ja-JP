---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 959a21339e9cc90c85edf83f1085d2b0d53c6728
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334117"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onenote/pages/{id}/content"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableArray *StreamList = [[NSMutableArray alloc] init];
MSGraphStream *Stream = [[MSGraphStream alloc] init];
[Stream setTarget:@"#para-id"];
[Stream setAction:@"insert"];
[Stream setPosition:@"before"];
[Stream setContent:@"<img src=\"image-url-or-part-name\" alt=\"image-alt-text\" />"];
[StreamList addObject: Stream];
MSGraphStream *Stream = [[MSGraphStream alloc] init];
[Stream setTarget:@"#list-id"];
[Stream setAction:@"append"];
[Stream setContent:@"<li>new-page-content</li>"];
[StreamList addObject: Stream];

NSError *error;
NSData *StreamData = [Stream getSerializedDataWithError:&error];
[urlRequest setHTTPBody:StreamData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```