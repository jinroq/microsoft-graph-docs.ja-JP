---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a312f79942e86f8cdd57a0d08b5313c93803b034
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459011"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .Request()
    .DeleteAsync();

```