---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e102b8e344382e52946d5d423ce742f0228e456
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461136"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADhMGAAA="]
    .Request()
    .GetAsync();

```