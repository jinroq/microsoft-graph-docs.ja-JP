---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c2269b70eaeb9b3cee6ebcfea6a1dc5f41c2d833
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327250"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getMailboxUsageMailboxCounts("D7")
    .buildRequest()
    .get();

```