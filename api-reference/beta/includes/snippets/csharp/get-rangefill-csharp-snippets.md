---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 92ac497eef7ebbbbd4facff0b6fcdeec824d16c8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874568"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Fill
    .Request()
    .GetAsync();

```