---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 533febab48f0d9dd0b94922ea5d835696096189e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359084"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessParticipantActivityUserCountsCollectionPage getSkypeForBusinessParticipantActivityUserCounts = graphClient.reports()
    .getSkypeForBusinessParticipantActivityUserCounts("D7")
    .buildRequest()
    .get();

```