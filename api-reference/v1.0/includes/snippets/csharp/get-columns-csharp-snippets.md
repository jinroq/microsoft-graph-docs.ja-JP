---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5de63092708e0e499dfe378602fffa38d5250322
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472294"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Request()
    .Skip(5)
    .Top(5)
    .GetAsync();

```