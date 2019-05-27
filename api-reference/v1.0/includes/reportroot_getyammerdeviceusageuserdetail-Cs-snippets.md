---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0e0ba3c3d861381e5e08b6fe5861997048760e26
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468810"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetYammerDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```