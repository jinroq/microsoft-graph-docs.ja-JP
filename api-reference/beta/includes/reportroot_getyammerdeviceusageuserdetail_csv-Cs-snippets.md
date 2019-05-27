---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6d644451770f4a3507c225656445cd4c14f3d4bc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482004"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerDeviceUsageUserDetail = await graphClient.Reports.GetYammerDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```