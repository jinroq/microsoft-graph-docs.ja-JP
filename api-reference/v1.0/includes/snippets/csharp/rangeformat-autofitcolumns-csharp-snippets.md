---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 159dabac73c5c292e6473e76106fec4d0ec50f0b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471799"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format
    .AutofitColumns()
    .Request()
    .PostAsync();

```