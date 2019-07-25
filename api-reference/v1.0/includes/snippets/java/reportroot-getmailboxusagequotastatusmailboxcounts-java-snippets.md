---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1b5dba05801e938d4b5a4971b42edf0a3eec5cdd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894366"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getMailboxUsageQuotaStatusMailboxCounts('D7')
    .buildRequest()
    .get();

```