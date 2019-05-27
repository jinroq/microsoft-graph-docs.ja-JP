---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ab8bde42fb4ca337230599efbf7c4da029724608
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{id}"]
    .Request()
    .DeleteAsync();

```