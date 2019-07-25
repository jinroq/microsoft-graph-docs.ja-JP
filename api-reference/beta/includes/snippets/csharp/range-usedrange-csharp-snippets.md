---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 18c6735a83768bb3f5fc67a57ccd0827ecde3088
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874693"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .UsedRange()
    .Request()
    .GetAsync();

```