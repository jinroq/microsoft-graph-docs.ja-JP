---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0724be357588cc1086d531cca4068ee7defed4cf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327209"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getMailboxUsageStorage("D7")
    .buildRequest()
    .get();

```