---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9d16c5f8babf8e57fcf1118721990891b96756c2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailActivityCounts('D7')
    .Request()
    .GetAsync();

```