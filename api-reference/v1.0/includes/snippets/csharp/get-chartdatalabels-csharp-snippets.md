---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2cb6d40afe7a5fdfef92775d8ac177b17dd72dff
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471900"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartDataLabels = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].DataLabels
    .Request()
    .GetAsync();

```