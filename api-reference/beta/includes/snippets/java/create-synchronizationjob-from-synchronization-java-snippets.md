---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e640ba29701aa7ad35abd49a9f20ec533c5a6739
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869327"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationJob synchronizationJob = new SynchronizationJob();
synchronizationJob.templateId = "BoxOutDelta";

graphClient.servicePrincipals("{id}").synchronization().jobs()
    .buildRequest()
    .post(synchronizationJob);

```