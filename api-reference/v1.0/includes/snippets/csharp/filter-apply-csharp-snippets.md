---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0438d26738016be4fe069efc547e3a8707b7746d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var criteria = new WorkbookFilterCriteria
{
    Criterion1 = "criterion1-value",
    Criterion2 = "criterion2-value",
    Color = "color-value",
    Operator = new String
    {
    },
    Icon = new WorkbookIcon
    {
        Set = "set-value",
        Index = 99
    },
    DynamicCriteria = "dynamicCriteria-value",
    Values = new Json
    {
    },
    FilterOn = "filterOn-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"].Filter
    .Apply(criteria)
    .Request()
    .PostAsync();

```