---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3e0cee3bc0aa608362aca4bb1727589bd3968308
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869348"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}")
    .pause()
    .buildRequest()
    .post();

```