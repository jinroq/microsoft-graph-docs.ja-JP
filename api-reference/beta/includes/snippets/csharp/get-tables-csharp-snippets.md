---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7e4a0ff78344c86f9424fe0c0b255c96f39c1352
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tables = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Tables
    .Request()
    .GetAsync();

```