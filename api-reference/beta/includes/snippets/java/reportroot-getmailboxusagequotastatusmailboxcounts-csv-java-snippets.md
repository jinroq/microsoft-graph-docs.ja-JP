---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e98310f0fd9758a314645657bea8da8ca31a6b4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873695"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailboxUsageQuotaStatusMailboxCountsCollectionPage getMailboxUsageQuotaStatusMailboxCounts = graphClient.reports()
    .getMailboxUsageQuotaStatusMailboxCounts('D7')
    .buildRequest()
    .get();

```