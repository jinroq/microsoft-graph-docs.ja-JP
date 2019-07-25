---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2c4b589d9dcd11e1319302a51296e09600d9549f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888817"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlan plannerPlan = graphClient.planner().plans("{plan-id}")
    .buildRequest()
    .get();

```