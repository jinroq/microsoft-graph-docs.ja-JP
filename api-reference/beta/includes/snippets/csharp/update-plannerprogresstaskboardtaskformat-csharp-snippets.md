---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7e5302f8679f701de554bbcf9369972d81e6c98d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720477"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerProgressTaskBoardTaskFormat = new PlannerProgressTaskBoardTaskFormat
{
    OrderHint = "A6673H Ejkl!"
};

await graphClient.Planner.Tasks["'id'"].ProgressTaskBoardFormat
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerProgressTaskBoardTaskFormat);

```