---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ad896836314fd9057630de6d8a3a811a62d9a7e1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873757"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailboxUsageMailboxCountsCollectionPage getMailboxUsageMailboxCounts = graphClient.reports()
    .getMailboxUsageMailboxCounts('D7')
    .buildRequest()
    .get();

```