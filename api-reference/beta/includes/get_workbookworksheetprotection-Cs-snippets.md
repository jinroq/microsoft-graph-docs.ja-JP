---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bc04092ab9760d7648b5104eface3bcda3d72454
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445064"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookWorksheetProtection = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Protection
    .Request()
    .GetAsync();

```