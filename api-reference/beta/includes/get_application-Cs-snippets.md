---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ed2bb061ef847d5cf854faa44ca94a936ae471f1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474059"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = await graphClient.Applications["{id}"]
    .Request()
    .GetAsync();

```