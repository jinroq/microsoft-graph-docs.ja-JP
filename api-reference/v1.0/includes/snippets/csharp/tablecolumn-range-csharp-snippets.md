---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8f6cd307a6c0d80e5202e471926f2db3118b77b3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .Range()
    .Request()
    .PostAsync();

```