---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b4a0a171d2d2a5cf15e9337cba369f355e1cb266
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891959"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucketTaskBoardTaskFormat plannerBucketTaskBoardTaskFormat = graphClient.planner().tasks("{task-id}").bucketTaskBoardFormat()
    .buildRequest()
    .get();

```