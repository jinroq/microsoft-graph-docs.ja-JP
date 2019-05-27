---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5c72a577f5cca9b31fa170abaa5624f9b06b05c3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447426"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRole = await graphClient.PrivilegedRoles["{id}"]
    .Request()
    .GetAsync();

```