---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5489dc5b30847d5009b909dc560db4aa8d52b73c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447048"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Fill
    .Request()
    .GetAsync();

```