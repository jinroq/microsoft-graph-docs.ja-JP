---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0fe153c463fdaf6bab58c14da62858723371af75
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873760"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageMailboxCounts = await graphClient.Reports
    .GetMailboxUsageMailboxCounts('D7')
    .Request()
    .GetAsync();

```