---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3a7c74fb0b6d9f3a305a508ab451083ec7aeb25e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445358"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = await graphClient.Security.TiIndicators["{id}"]
    .Request()
    .GetAsync();

```