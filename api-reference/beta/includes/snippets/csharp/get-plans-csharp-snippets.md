---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3dac820a91b45274c6798ceedb1c844f387b4e79
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720691"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = await graphClient.Me.Planner.Plans
    .Request()
    .GetAsync();

```