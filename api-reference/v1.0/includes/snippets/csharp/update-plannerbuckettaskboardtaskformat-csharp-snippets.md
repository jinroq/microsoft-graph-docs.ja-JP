---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 813453216b2404bd81c1f18f1b5da0d23ba1801d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731779"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucketTaskBoardTaskFormat = new PlannerBucketTaskBoardTaskFormat
{
    OrderHint = "A6673H Ejkl!"
};

await graphClient.Planner.Tasks["{task-id}"].BucketTaskBoardFormat
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerBucketTaskBoardTaskFormat);

```