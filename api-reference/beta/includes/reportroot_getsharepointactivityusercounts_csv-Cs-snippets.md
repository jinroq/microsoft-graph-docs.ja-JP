---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7d980e3e1877a7caa6e673a1917fb7237c56c1d0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440752"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityUserCounts = await graphClient.Reports.GetSharePointActivityUserCounts('D7')
    .Request()
    .GetAsync();

```