---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bc28759d2c021ee8556f06b9bdd5770c5ca91b95
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736061"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applyTo = "applyTo-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Clear(applyTo)
    .Request()
    .PostAsync();

```