---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f0c1f55373473cdc94cd9d1265494b32909e6df3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459506"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.ContactFolders["{id}"]
    .Request()
    .DeleteAsync();

```