---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fe240f739a2484aaa5ff728f0dc99bebea6c982d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467833"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartTitle = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Title
    .Request()
    .GetAsync();

```