---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3a5ecc91497201151a6403be84b244aad125d5a8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728161"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = "shift-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Insert(shift)
    .Request()
    .PostAsync();

```