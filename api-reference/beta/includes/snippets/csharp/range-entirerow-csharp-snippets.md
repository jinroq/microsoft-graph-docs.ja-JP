---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e2813b0a3fec9906b201c6722801373a2bad6154
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486492"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().EntireRow()
    .Request()
    .GetAsync();

```