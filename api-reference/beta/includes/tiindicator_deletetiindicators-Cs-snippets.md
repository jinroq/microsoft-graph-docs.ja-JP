---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 691b4ae1633ce91fa60e274e9743edd52ef72755
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469322"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<String>()
{
    "id-value1",
    "id-value2"
};

await graphClient.Security.TiIndicators
    .DeleteTiIndicators(value)
    .Request()
    .PostAsync();

```