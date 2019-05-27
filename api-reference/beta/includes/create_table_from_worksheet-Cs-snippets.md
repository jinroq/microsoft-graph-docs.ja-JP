---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4f70f5401ebb81b744b73cf551f1c7fa8938d0c0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439415"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "";

var hasHeaders = false;

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Tables
    .Add(address,hasHeaders)
    .Request()
    .PostAsync();

```