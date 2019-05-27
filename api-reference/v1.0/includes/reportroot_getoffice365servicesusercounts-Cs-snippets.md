---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9fa55573bb9121f2a59e2958783715de5de01e53
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478721"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365ServicesUserCounts('D7')
    .Request()
    .GetAsync();

```