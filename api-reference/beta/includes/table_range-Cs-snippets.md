---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 19aaa62f26007d0a1ae2e6ba64f8c04687305248
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465833"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .Range()
    .Request()
    .PostAsync();

```