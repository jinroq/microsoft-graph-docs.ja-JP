---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9e37f987c53fcfee60728e176ff77019c07e0a34
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320319"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerDeviceUsageDistributionUserCounts("D7")
    .Request()
    .GetAsync();

```