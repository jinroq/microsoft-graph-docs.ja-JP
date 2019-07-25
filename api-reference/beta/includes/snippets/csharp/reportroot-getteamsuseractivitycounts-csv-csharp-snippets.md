---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4bfb3ac1b274eac5bb5431f7b1e514eeb876786c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityCounts = await graphClient.Reports
    .GetTeamsUserActivityCounts('D7')
    .Request()
    .GetAsync();

```