---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: acc1d6e1d915e28fde5380293115b46a70caaab0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864876"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean all = True;

String clientContext = "clientContext-value";

graphClient.app().calls("{id}")
    .cancelMediaProcessing(all,clientContext)
    .buildRequest()
    .post();

```