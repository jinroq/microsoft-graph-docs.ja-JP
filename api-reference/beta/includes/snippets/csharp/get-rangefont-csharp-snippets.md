---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1fa4b22b9c9ccedd5da8e9d0bc37c750bafd0975
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874497"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Font
    .Request()
    .GetAsync();

```