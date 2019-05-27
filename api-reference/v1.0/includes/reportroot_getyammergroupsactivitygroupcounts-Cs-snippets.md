---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ec38d005bef75ce6eefec1ffb3b358899fe653de
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468782"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetYammerGroupsActivityGroupCounts('D7')
    .Request()
    .GetAsync();

```