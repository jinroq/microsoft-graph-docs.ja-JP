---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 89bd1e7d34c19f2d0ce21d7f0974e86d79c02d40
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887053"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerProgressTaskBoardTaskFormat plannerProgressTaskBoardTaskFormat = new PlannerProgressTaskBoardTaskFormat();
plannerProgressTaskBoardTaskFormat.orderHint = "A6673H Ejkl!";

graphClient.planner().tasks("{task-id}").progressTaskBoardFormat()
    .buildRequest( requestOptions )
    .patch(plannerProgressTaskBoardTaskFormat);

```