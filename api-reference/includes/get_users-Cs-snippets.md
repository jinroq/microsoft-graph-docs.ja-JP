---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 711e0ffeabd73b0ce6c8873fc4da7bd394f7bb39
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843487"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Users["{user-id}"]
    .Request()
    .GetAsync();

```