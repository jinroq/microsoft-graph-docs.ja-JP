---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5a12d58a26bbbabaa9a3d2470068efb37569eb75
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var persistChanges = true;

await graphClient.Me.Drive.Items["{id}"].Workbook
    .CreateSession(this,persistChanges)
    .Request()
    .PostAsync();

```