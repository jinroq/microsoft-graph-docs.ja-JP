---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3b3f18fd5b32dc9299a9a7c65dedf9aa6256be57
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870762"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean notifyTeam = True;

int startDateTime = 10/8/2018 12:00:00 AM;

int endDateTime = 10/15/2018 12:00:00 AM;

graphClient.teams("{teamId}").schedule()
    .share(notifyTeam,startDateTime,endDateTime)
    .buildRequest()
    .post();

```