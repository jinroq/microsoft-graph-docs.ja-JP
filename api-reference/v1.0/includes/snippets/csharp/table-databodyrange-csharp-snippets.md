---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4d049104c64d355acb7ba96ee5101fa534914a87
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723121"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .DataBodyRange()
    .Request()
    .PostAsync();

```