---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 266f88b28dee27a1ba20808d0261bd20850f46f9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872623"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageSiteCounts = await graphClient.Reports
    .GetSharePointSiteUsageSiteCounts('D7')
    .Request()
    .GetAsync();

```