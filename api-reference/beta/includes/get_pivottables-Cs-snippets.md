---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1a2039ff3ec1cc784ebc84df16a29e2c9bee7d6c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447811"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pivotTables = await graphClient.Drive.Root.Workbook.Worksheets["{id}"].PivotTables
    .Request()
    .GetAsync();

```