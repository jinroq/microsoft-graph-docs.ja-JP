---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1818ce89be1c1dc1a1da2c2b72ec7bf957083362
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872820"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointActivityUserCountsCollectionPage getSharePointActivityUserCounts = graphClient.reports()
    .getSharePointActivityUserCounts('D7')
    .buildRequest()
    .get();

```