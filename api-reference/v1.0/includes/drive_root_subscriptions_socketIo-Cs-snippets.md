---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 21ab5b4454c31f3299eb676dfbfe6d96c066309b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457959"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = await graphClient.Me.Drive.Root.Subscriptions["socketIo"]
    .Request()
    .GetAsync();

```