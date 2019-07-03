---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0d0d3c5dfbd4021391cc66bf909d856b22109763
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513444"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Sort
    .Clear()
    .Request()
    .PostAsync();

```