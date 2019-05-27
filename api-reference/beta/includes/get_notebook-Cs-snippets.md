---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 672ec71879101810db62196e93b61fa83f4e1d77
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448392"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebook = await graphClient.Me.Onenote.Notebooks["{id}"]
    .Request()
    .GetAsync();

```