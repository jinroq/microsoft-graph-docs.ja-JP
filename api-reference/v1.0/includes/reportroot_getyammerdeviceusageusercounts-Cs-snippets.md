---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e8e9e9fce038a41558238d6dde6972834da395b1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469063"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetYammerDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```