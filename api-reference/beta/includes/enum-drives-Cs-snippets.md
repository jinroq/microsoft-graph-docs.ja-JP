---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9a094c980539f75a2d663cecc77cbe2f00c28479
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436867"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Me.Drives
    .Request()
    .GetAsync();

```