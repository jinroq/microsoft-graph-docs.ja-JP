---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dcdadfc1f0ecea66573573b9e0ae02da33c3dfc6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471111"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerAssignedToTaskBoardTaskFormat = await graphClient.Planner.Tasks["{task-id}"].AssignedToTaskBoardFormat
    .Request()
    .GetAsync();

```