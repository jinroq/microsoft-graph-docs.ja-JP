---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 87bf8dcd63b4651745d9db26b8e76afa8c424dcf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874917"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .EntireColumn()
    .Request()
    .GetAsync();

```