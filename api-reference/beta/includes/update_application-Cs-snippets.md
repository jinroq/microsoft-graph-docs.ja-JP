---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 66b16f590e48ee5c9c9bce0b5f79174eae968390
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    AllowPublicClient = false,
    DisplayName = "New display name"
};

await graphClient.Applications["{id}"]
    .Request()
    .UpdateAsync(application);

```