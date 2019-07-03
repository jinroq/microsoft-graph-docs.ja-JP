---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3a7c74fb0b6d9f3a305a508ab451083ec7aeb25e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527024"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = await graphClient.Security.TiIndicators["{id}"]
    .Request()
    .GetAsync();

```