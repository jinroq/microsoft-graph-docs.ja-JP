---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 217f31582fafdb221d6f537ed9de543a53e31cbf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fields = new List<WorkbookSortField>()
{
    new WorkbookSortField
    {
        Key = 99,
        SortOn = "sortOn-value",
        Ascending = true,
        Color = "color-value",
        DataOption = "dataOption-value",
        Icon = new WorkbookIcon
        {
            Set = "set-value",
            Index = 99
        }
    }
};

var matchCase = true;

var hasHeaders = true;

var orientation = "orientation-value";

var method = "method-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Sort
    .Apply(fields,matchCase,hasHeaders,orientation,method)
    .Request()
    .PostAsync();

```