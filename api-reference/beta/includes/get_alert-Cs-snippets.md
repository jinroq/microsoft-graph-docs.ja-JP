---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d4df16ee11685a1b4d429214ba577f4c26eef537
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474157"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = await graphClient.Security.Alerts["{id}"]
    .Request()
    .GetAsync();

```