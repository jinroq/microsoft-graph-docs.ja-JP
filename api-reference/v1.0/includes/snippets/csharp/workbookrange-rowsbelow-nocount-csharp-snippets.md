---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9871f6b52e8cfd02f68d7b9fde19dcf034323d40
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740578"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].Range().RowsBelow()
    .Request()
    .GetAsync();

```