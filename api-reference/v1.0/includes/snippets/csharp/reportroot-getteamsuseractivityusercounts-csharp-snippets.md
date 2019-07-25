---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 123883f6a961a5e2d9388087b61e6b82c977bdec
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886659"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsUserActivityUserCounts('D7')
    .Request()
    .GetAsync();

```