---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8e7f0b5f8e09c5a2a5f1dd944cb6bcdb17c15287
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739752"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Sort
    .Reapply()
    .Request()
    .PostAsync();

```