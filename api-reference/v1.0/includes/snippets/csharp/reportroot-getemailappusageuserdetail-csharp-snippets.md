---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e8c539497cfbd14b0c7383b5c31dddc42e0ab8c9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886342"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailAppUsageUserDetail('D7')
    .Request()
    .GetAsync();

```