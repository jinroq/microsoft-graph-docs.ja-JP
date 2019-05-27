---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b6e65b1da384ecf223b7b2746e8ef654846b748c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoles["{id}"]
    .SelfDeactivate()
    .Request()
    .PostAsync();

```