---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ab63d70b639c3a4b5ff83bf207f9a41f6d0c7e05
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734748"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTaskDetails = await graphClient.Planner.Tasks["{task-id}"].Details
    .Request()
    .GetAsync();

```