---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9c6999c721650c195c06a974b3edac1eebfa2d7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736030"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Column(5)
    .Request()
    .GetAsync();

```