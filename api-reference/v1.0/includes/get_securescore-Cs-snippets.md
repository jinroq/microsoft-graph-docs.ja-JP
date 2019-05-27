---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 460bc93c7e2ebcde55a74533e6849be06b62958d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481633"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScore = await graphClient.Security.SecureScores["{id}"]
    .Request()
    .GetAsync();

```