---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 100e28b47682812022e84bd1f4aca665956c1df0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871736"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsUserActivityCountsCollectionPage getTeamsUserActivityCounts = graphClient.reports()
    .getTeamsUserActivityCounts('D7')
    .buildRequest()
    .get();

```