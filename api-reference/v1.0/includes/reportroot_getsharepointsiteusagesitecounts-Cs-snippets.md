---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a5a3ba64b0fe97f596f0e36673fdb74ac0ea1c70
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointSiteUsageSiteCounts('D7')
    .Request()
    .GetAsync();

```