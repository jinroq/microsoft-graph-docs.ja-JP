---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d697243d36debb29fb2a13093f5c98e4f05a0cd3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720496"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlanDetails = new PlannerPlanDetails
{
    SharedWith = new PlannerUserIds
    {
        6463a5ce-2119-4198-9f2a-628761df4a62 = true,
        D95e6152-f683-4d78-9ff5-67ad180fea4a = false
    },
    CategoryDescriptions = new PlannerCategoryDescriptions
    {
        Category1 = "Indoors",
        Category3 = null
    }
};

await graphClient.Planner.Plans["xqQg5FS2LkCp935s-FIFm2QAFkHM"].Details
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerPlanDetails);

```