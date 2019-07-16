---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ab8dd3fdcb386d6c07833cd97144c59f5144f2ba
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735931"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().EntireColumn()
    .Request()
    .GetAsync();

```