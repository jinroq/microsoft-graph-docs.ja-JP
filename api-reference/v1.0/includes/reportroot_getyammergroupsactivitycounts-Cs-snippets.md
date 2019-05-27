---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 27c960a449ad474e62144ce4212ae660c2dce01b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468789"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetYammerGroupsActivityCounts('D7')
    .Request()
    .GetAsync();

```