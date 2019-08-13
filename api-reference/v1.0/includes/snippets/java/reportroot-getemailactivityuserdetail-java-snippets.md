---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 94a8a17ea70af05530f87bcc36cecc1338f04218
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327404"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailActivityUserDetail("D7")
    .buildRequest()
    .get();

```