---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 26f154290351fe99f3c428b61945ab9219b1bc7f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876447"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlan plannerPlan = graphClient.planner().plans("'id'")
    .buildRequest()
    .get();

```