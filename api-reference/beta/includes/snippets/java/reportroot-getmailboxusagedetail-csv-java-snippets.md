---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a22aad0b4aa73acd67acd221df03441553d49cf7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360578"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailboxUsageDetailCollectionPage getMailboxUsageDetail = graphClient.reports()
    .getMailboxUsageDetail("D7")
    .buildRequest()
    .get();

```