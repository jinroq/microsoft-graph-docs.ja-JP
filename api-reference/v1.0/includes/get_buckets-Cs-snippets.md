---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9c80211545ca96b6afd85c4b89e2894dff26ec13
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469770"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = await graphClient.Planner.Plans["{plan-id}"].Buckets
    .Request()
    .GetAsync();

```