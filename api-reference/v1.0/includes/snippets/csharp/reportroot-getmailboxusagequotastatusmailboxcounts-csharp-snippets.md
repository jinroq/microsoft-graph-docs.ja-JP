---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 32dfe7c05b363b39c5ca60534cf027c1c9ada637
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894365"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetMailboxUsageQuotaStatusMailboxCounts('D7')
    .Request()
    .GetAsync();

```