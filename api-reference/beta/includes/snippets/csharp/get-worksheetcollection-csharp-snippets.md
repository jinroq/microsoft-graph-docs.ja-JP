---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 65bc190f85fab212ecdebf1f6aa3444f64c88588
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723639"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var worksheets = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets
    .Request()
    .GetAsync();

```