---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f590bcecd62e89f13c143fc9ea20c4e599a19b55
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884257"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
    .UsedRange()
    .Request()
    .GetAsync();

```