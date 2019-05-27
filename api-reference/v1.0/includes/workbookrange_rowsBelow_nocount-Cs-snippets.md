---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9871f6b52e8cfd02f68d7b9fde19dcf034323d40
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450504"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].Range().RowsBelow()
    .Request()
    .GetAsync();

```