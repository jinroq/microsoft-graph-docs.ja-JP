---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e4f7d16293f55c6dc6ca5e725a72222c0e0a4ef
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504356"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = new Int32
{
};

var values = new List<Json>()
{
    new Json
    {
    }
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Add(index,values,name)
    .Request()
    .PostAsync();

```