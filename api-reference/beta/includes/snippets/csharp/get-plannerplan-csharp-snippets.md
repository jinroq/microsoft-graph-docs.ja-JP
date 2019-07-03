---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6bdcf26068766695076804da73b14c44a2e343ec
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlan = await graphClient.Planner.Plans["'id'"]
    .Request()
    .GetAsync();

```