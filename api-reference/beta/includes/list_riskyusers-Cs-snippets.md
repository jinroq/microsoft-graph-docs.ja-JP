---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f2bcd041605a03129da2c1dd23f7c33069dac493
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444287"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUsers = await graphClient.RiskyUsers
    .Request()
    .GetAsync();

```