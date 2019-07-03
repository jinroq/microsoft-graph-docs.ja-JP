---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1d11751ef93790d7a3f1c160e673a27441f14121
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471814"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeSort = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Sort
    .Request()
    .GetAsync();

```