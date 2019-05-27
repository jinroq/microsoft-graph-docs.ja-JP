---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6b17db6383c198263a968dd8dd8917f076e258b2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Users["{userId}"].Drives
    .Request()
    .GetAsync();

```