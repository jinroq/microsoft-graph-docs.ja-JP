---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: da0fb3eab26035e101a2d9ca7db009bd3ba7cb48
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889681"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range('A1:Z10')
    .VisibleView()
    .Range()
    .Request()
    .GetAsync();

```