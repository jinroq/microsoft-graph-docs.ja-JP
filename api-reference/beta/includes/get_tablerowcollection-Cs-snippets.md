---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 19979e7c97b22748181f91c40244d0472c8c1e33
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows
    .Request()
    .GetAsync();

```