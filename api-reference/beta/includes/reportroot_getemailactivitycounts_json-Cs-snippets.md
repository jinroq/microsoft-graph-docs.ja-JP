---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: db05a1a1279e1647d4d1114a2016756a0658d9c4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442411"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailActivityCounts = await graphClient.Reports.GetEmailActivityCounts('D7')
    .Request()
    .GetAsync();

```