---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5709bb98d40f0b696796a69e9807afd949b36ec6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876643"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucket plannerBucket = new PlannerBucket();
plannerBucket.name = "Advertising";
plannerBucket.planId = "xqQg5FS2LkCp935s-FIFm2QAFkHM";
plannerBucket.orderHint = " !";

graphClient.planner().buckets()
    .buildRequest()
    .post(plannerBucket);

```