---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8a371f95e2f0e2e8af2958c9ec7012a40b421c04
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetYammerGroupsActivityDetail('D7')
    .Request()
    .GetAsync();

```