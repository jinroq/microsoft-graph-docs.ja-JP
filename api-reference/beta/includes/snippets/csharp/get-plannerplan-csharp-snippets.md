---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 27b554c11b3ef25406c40be17b0f99d18945f1d6
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlan = await graphClient.Planner.Plans["{id}"]
    .Request()
    .GetAsync();

```