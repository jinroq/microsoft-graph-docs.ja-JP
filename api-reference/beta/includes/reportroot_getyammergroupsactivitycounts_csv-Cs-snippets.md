---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d274dee65cd5f5821bd186b1926bde3270c35aaf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481955"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerGroupsActivityCounts = await graphClient.Reports.GetYammerGroupsActivityCounts('D7')
    .Request()
    .GetAsync();

```