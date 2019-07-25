---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c35621c97eb281d806344fa0dbbea94a85915b6c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881247"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerGroupsActivityCounts('D7')
    .buildRequest()
    .get();

```