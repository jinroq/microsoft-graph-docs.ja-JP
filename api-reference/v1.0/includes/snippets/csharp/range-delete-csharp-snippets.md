---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 20a18b4fb0e9d25b67b552b8c6277b66d79171a9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735952"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = "shift-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Delete(shift)
    .Request()
    .PostAsync();

```