---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2e00a52aaa8d68b3bd1b75249788de1eedfb86a9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447230"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programControls = await graphClient.ProgramControls
    .Request()
    .GetAsync();

```