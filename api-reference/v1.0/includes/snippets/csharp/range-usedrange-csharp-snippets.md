---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8e72011a83316b20240708a5d9a6c8771c0bc72b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471812"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().UsedRange()
    .Request()
    .GetAsync();

```