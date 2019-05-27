---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ac0a2aeb9973d9d31205cb7cd61a0c5b6c191e25
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOneDriveUsageFileCounts('D7')
    .Request()
    .GetAsync();

```