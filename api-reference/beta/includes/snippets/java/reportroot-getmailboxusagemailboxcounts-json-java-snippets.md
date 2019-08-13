---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 54d2bc512f61d22ffa61e5870f9286319253010d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308693"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailboxUsageMailboxCountsCollectionPage getMailboxUsageMailboxCounts = graphClient.reports()
    .getMailboxUsageMailboxCounts("D7")
    .buildRequest()
    .get();

```