---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cbb7021603a2dca5c41225166ac911e2cce027d9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875200"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.onPremisesPublishingProfiles("provisioning").publishedResources("1234b780-965f-4149-85c5-a8c73e58b67d").agentGroups("8832388F-3814-4952-B288-FFB62081FE25").reference()
    .buildRequest()
    .delete();

```