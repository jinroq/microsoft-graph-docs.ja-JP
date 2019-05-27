---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 881ec7bac57269dbf90029c04bc7ea76988cf56c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439240"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.App.Calls["{id}"]
    .Request()
    .DeleteAsync();

```