---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c1b167466911c8954afa9beceb9984e6b6fe48a0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sites = await graphClient.Sites
    .Request()
    .GetAsync();

```