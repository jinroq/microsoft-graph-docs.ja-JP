---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ec06316e47229b48b97e487aafa09c42b82cd437
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716085"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsAfter(count)
    .Request()
    .PostAsync();

```