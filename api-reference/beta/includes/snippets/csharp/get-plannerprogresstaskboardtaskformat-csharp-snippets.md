---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ad62b66f308c9da0b6ffad1ef297dba173839846
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485067"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerProgressTaskBoardTaskFormat = await graphClient.Planner.Tasks["'id'"].ProgressTaskBoardFormat
    .Request()
    .GetAsync();

```