---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a0cde933cae57d59449028b26783341ff43db821
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878534"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.onPremisesPublishingProfiles("provisioning").agentGroups("8832388F-3814-4952-B288-FFB62081FE25")
    .buildRequest()
    .delete();

```