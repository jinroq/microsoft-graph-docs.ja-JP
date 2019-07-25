---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4783eed37e43ebf4d077afab72ce6460fbff94bb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876207"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Planner.All
    .Delta()
    .Request()
    .GetAsync();

```