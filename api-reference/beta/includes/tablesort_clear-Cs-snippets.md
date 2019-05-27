---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0d0d3c5dfbd4021391cc66bf909d856b22109763
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454377"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Sort
    .Clear()
    .Request()
    .PostAsync();

```