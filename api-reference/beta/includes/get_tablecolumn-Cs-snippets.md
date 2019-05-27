---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1eeff8698f429a743ffc3c3fb0ae292905daba35
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445666"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableColumn = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .Request()
    .GetAsync();

```