---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c6e58cd786b2cbf40045c728a13a0f63dfe47344
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715958"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "address-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
    .Range()
    .Request()
    .PostAsync();

```