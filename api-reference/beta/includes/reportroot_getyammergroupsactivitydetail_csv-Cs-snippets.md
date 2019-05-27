---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f39fa5a476d479c211249d9eb2c85bb1ceef48a5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481885"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerGroupsActivityDetail = await graphClient.Reports.GetYammerGroupsActivityDetail('D7')
    .Request()
    .GetAsync();

```