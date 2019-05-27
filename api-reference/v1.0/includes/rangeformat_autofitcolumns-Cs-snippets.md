---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 159dabac73c5c292e6473e76106fec4d0ec50f0b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469640"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format
    .AutofitColumns()
    .Request()
    .PostAsync();

```