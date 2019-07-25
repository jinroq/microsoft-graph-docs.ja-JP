---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 513b1154144275ea6449ea167c8a7fc4873a6389
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876206"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerDeltaDeltaCollectionPage delta = graphClient.me().planner().all()
    .delta()
    .buildRequest()
    .get();

```