---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 170e4175d24833cf2e3e89d55df871297dcdc05b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471889"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartPoint = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Series["{series-id}"].Points["{point-id}"]
    .Request()
    .GetAsync();

```