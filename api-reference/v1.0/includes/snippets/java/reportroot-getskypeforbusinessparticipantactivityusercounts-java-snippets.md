---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0c121e7b930f4d7b2198f19d4c85cb5697482765
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320675"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessParticipantActivityUserCounts("D7")
    .buildRequest()
    .get();

```