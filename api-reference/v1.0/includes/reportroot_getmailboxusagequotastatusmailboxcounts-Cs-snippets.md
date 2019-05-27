---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3478bc712cb684c2388720d5547361626be29ea9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434599"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetMailboxUsageQuotaStatusMailboxCounts('D7')
    .Request()
    .GetAsync();

```