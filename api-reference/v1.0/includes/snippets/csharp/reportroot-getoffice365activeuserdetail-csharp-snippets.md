---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c38d257f3694a33ee35342e0fbe3667e785c659a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894002"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365ActiveUserDetail('D7')
    .Request()
    .GetAsync();

```