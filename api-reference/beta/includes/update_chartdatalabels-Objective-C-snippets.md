---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c57091367acc0572eb1139bb31f4f39ba026f557
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334567"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartDataLabels *workbookChartDataLabels = [[MSGraphWorkbookChartDataLabels alloc] init];
[workbookChartDataLabels setPosition:@"position-value"];
[workbookChartDataLabels setShowValue: true];
[workbookChartDataLabels setShowSeriesName: true];
[workbookChartDataLabels setShowCategoryName: true];
[workbookChartDataLabels setShowLegendKey: true];

NSError *error;
NSData *workbookChartDataLabelsData = [workbookChartDataLabels getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartDataLabelsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```