---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9c6999c721650c195c06a974b3edac1eebfa2d7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452722"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Column(5)
    .Request()
    .GetAsync();

```