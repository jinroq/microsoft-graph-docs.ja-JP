---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 97f1735ba961191bb70da4c506c3af15c8027a8f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .TotalRowRange()
    .Request()
    .PostAsync();

```