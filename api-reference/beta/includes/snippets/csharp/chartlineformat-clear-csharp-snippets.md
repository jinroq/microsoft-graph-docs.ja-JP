---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0e7ae64c0e38fcd2c576112853f8744458cade25
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708071"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.SeriesAxis.Format.Line
    .Clear()
    .Request()
    .PostAsync();

```