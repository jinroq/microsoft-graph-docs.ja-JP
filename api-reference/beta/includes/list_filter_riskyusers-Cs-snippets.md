---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7d64a8b20e9d6be70f8937dc31142a085d4fdee3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444315"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUsers = await graphClient.RiskyUsers
    .Request()
    .Filter("riskLevel eq microsoft.graph.riskLevel'medium'")
    .GetAsync();

```