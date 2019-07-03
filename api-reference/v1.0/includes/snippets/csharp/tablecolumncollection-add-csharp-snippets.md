---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c37f87c5ee87c32ea44f4fb5977f9079f4863ce8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496156"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = 3;

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