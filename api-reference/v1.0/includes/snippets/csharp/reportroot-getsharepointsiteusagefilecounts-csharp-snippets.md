---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 285b7e45cd16680268208d5b5c8c5bad04c87034
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893433"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageFileCounts('D7')
    .Request()
    .GetAsync();

```