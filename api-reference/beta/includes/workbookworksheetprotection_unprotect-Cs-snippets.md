---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 72520adae193e0ab3182c33c1b438e3a8986454f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var password = "password-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Protection
    .Unprotect()
    .Request()
    .PostAsync();

```