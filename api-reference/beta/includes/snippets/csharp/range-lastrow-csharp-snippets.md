---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e3e3572bf13e8015fb796637d5a30dbd42a5be42
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874752"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .LastRow()
    .Request()
    .GetAsync();

```