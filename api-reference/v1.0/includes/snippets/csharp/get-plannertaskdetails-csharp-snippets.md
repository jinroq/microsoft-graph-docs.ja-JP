---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ab63d70b639c3a4b5ff83bf207f9a41f6d0c7e05
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471100"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTaskDetails = await graphClient.Planner.Tasks["{task-id}"].Details
    .Request()
    .GetAsync();

```