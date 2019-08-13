---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 89b8316b536f2ef1a195d16d299bd7cd2eb06e25
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327271"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getMailboxUsageQuotaStatusMailboxCounts("D7")
    .buildRequest()
    .get();

```