---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8ade44bdd9afe47d55ccbe8bc1d1752017ddbfc9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873946"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageAppsUserCounts = await graphClient.Reports
    .GetEmailAppUsageAppsUserCounts('D7')
    .Request()
    .GetAsync();

```