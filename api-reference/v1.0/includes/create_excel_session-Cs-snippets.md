---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5a12d58a26bbbabaa9a3d2470068efb37569eb75
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454363"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var persistChanges = true;

await graphClient.Me.Drive.Items["{id}"].Workbook
    .CreateSession(this,persistChanges)
    .Request()
    .PostAsync();

```