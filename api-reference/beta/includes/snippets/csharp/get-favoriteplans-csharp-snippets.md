---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 52811b736c4a4016c221b341a721b5d75c7ba935
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503739"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var favoritePlans = await graphClient.Me.Planner.FavoritePlans
    .Request()
    .GetAsync();

```