---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a71ab851589bdd7d0259d5b521f22bddeb8363d4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857222"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Column(5)
    .Request()
    .GetAsync();

```