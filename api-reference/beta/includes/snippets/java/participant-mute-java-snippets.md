---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca17e66b1771b61cc9569a5fc0375c425d27cde9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877049"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

graphClient.app().calls("{id}").participants("{id}")
    .mute(clientContext)
    .buildRequest()
    .post();

```