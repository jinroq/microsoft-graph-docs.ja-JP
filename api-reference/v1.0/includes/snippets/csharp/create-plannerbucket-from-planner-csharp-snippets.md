---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c1f49cfe4fc6c0f3bb63b7e7cbcaeb078940d05b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731541"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucket = new PlannerBucket
{
    Name = "Advertising",
    PlanId = "xqQg5FS2LkCp935s-FIFm2QAFkHM",
    OrderHint = " !"
};

await graphClient.Planner.Buckets
    .Request()
    .AddAsync(plannerBucket);

```