---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4416d7d1c02dfa07a0573c39228c252c1122421e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885950"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerDeviceUsageDistributionUserCounts('D7')
    .Request()
    .GetAsync();

```