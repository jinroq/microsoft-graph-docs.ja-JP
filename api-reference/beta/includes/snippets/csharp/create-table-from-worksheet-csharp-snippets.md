---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4f70f5401ebb81b744b73cf551f1c7fa8938d0c0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723616"
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