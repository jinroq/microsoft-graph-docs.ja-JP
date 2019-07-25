---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2c37f0283ded5d22785ca2b92108bdba45faad1f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871281"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerGroupsActivityGroupCountsCollectionPage getYammerGroupsActivityGroupCounts = graphClient.reports()
    .getYammerGroupsActivityGroupCounts('D7')
    .buildRequest()
    .get();

```