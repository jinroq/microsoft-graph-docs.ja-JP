---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 02727a1c2499e558f1d2b6584ccf7a2c4f55a9b7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"]
    .Request()
    .DeleteAsync();

```