---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 39548837e8e033276140337c3ff72d35febf2db7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439050"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"]
    .Request()
    .DeleteAsync();

```