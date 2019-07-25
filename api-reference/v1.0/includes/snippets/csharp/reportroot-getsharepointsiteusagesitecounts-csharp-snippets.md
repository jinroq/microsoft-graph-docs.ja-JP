---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 709b55d609e0c57fd23b21212df4e1494cfad48b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893384"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageSiteCounts('D7')
    .Request()
    .GetAsync();

```