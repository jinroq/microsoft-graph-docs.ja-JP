---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 50d748b18a34fa01d6a780c9a7df764bd26e17b3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327239"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getMailboxUsageDetail("D7")
    .buildRequest()
    .get();

```