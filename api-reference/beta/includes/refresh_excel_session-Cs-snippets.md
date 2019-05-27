---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a37fccafdc8707fd5635da7b2cfb97f9fe54440b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442551"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook
    .RefreshSession(this)
    .Request()
    .Header("workbook-session-id","{session-id}")
    .PostAsync();

```