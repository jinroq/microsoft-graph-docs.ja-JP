---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b27a9f0711759f53e42f7501a4f95c32128fb4eb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714182"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{id}"]
    .DismissReminder()
    .Request()
    .PostAsync();

```