---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5704ec2ca1657394506a10639334462ed458b7a9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735974"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Cell(5,6)
    .Request()
    .GetAsync();

```