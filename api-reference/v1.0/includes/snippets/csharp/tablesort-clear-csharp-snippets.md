---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0d0d3c5dfbd4021391cc66bf909d856b22109763
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739795"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Sort
    .Clear()
    .Request()
    .PostAsync();

```