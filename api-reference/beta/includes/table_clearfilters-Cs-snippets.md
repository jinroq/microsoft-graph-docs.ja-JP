---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e64bac722ba797220ed4998ece71ff952bebcc78
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .ClearFilters()
    .Request()
    .PostAsync();

```