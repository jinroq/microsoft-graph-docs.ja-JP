---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 52811b736c4a4016c221b341a721b5d75c7ba935
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720410"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var favoritePlans = await graphClient.Me.Planner.FavoritePlans
    .Request()
    .GetAsync();

```