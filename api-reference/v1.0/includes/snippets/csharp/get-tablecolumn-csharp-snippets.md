---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1eeff8698f429a743ffc3c3fb0ae292905daba35
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableColumn = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .Request()
    .GetAsync();

```