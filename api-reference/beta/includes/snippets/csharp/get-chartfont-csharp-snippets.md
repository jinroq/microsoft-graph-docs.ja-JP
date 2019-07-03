---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3e6420d528d7058fd95327db1afb7faf0f9f3e4c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526640"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartFont = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis.Format.Font
    .Request()
    .GetAsync();

```