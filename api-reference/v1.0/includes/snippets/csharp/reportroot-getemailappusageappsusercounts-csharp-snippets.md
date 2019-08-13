---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6339274f1581ba0d8676b50d46dcb3147c1907e9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327378"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailAppUsageAppsUserCounts("D7")
    .Request()
    .GetAsync();

```