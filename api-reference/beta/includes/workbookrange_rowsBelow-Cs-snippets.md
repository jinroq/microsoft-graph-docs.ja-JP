---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c58224e5526d0b829237f782c169dfd0c1c7e0f3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453209"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsBelow(count)
    .Request()
    .PostAsync();

```