---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c0b1818df37fb534f6215520fd528ddf5142dfef
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440563"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetEmailAppUsageUserDetail('D7')
    .Request()
    .GetAsync();

```