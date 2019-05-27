---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 03a62fc655cbbdab147da727cd99a0246a542319
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458672"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.MasterCategories["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"]
    .Request()
    .DeleteAsync();

```