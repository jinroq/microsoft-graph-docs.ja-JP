---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 20efc75d238e06b807e50b22e2332f2974900902
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463234"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = await graphClient.GroupSettings["{id}"]
    .Request()
    .GetAsync();

```