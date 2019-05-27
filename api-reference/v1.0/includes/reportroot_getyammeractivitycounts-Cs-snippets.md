---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c43bc08cc299683ce64bde6756f6789e64311893
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455899"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetYammerActivityCounts('D7')
    .Request()
    .GetAsync();

```