---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bc04092ab9760d7648b5104eface3bcda3d72454
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723561"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookWorksheetProtection = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Protection
    .Request()
    .GetAsync();

```