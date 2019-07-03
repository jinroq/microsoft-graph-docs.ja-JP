---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 65d7d2a966985f15f0d693a796986f771d9dc41f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485245"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var name = "test7";

var formula = "=SUM(Sheet2!$A$1+Sheet2!$A$2)";

var comment = "Comment for the named item";

await graphClient.Me.Drive.Items["{id}"].Workbook.Names
    .AddFormulaLocal(name,formula,comment)
    .Request()
    .PostAsync();

```