---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 240b686fd23e8a215156c3e5d3a9c94b429cb4cc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868396"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Schedule schedule = new Schedule();
schedule.enabled = true;
schedule.timeZone = "America/Chicago";

graphClient.teams("{teamId}").schedule()
    .buildRequest()
    .put(schedule);

```