---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2621d5fc0bbf6b6509bcf3b340b38217354b5b19
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["{object-id}"]
    .Restore()
    .Request()
    .PostAsync();

```