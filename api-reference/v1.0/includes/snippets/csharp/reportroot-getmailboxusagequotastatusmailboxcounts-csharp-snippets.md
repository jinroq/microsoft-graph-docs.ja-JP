---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4714b5d416961e5d5b83464eeabfee912930cad7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327272"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetMailboxUsageQuotaStatusMailboxCounts("D7")
    .Request()
    .GetAsync();

```