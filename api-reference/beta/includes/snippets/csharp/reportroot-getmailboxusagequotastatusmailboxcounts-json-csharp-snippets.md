---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fcc95277dc7b74b9345877280c2a420e4aed6795
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873693"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageQuotaStatusMailboxCounts = await graphClient.Reports
    .GetMailboxUsageQuotaStatusMailboxCounts('D7')
    .Request()
    .GetAsync();

```