---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 384141283eb8690b83cb3fde8db545bec2b56a44
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733894"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Unmerge()
    .Request()
    .PostAsync();

```