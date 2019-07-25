---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ebf3d761c620f73773efaff47edcd5be0f1dbd27
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894387"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getMailboxUsageMailboxCounts('D7')
    .buildRequest()
    .get();

```