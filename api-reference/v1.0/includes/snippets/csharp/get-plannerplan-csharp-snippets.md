---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 12065c13a0c7e6ba103025ff3cd6cc28bb8c43fc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471105"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlan = await graphClient.Planner.Plans["{plan-id}"]
    .Request()
    .GetAsync();

```