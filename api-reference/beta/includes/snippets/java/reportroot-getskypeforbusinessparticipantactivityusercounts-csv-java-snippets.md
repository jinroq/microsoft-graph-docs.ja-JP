---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d0c65263af40601804b4130fa86d6e1698728e0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872037"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessParticipantActivityUserCountsCollectionPage getSkypeForBusinessParticipantActivityUserCounts = graphClient.reports()
    .getSkypeForBusinessParticipantActivityUserCounts('D7')
    .buildRequest()
    .get();

```