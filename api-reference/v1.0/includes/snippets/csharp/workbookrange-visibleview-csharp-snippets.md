---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0e88817edda1e3781cfdbc0db36e0d3a0c34e3e5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeView = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].Range('A1:Z10').VisibleView()
    .Request()
    .GetAsync();

```