---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 65cd336650b64d9a6f4cbdad8145675fb314eb2d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358788"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsUserActivityUserCountsCollectionPage getTeamsUserActivityUserCounts = graphClient.reports()
    .getTeamsUserActivityUserCounts("D7")
    .buildRequest()
    .get();

```