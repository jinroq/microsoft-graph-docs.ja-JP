---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fbd7a5e75168e4d4a30f5b9969ee2a1ecd11d0cf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358549"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerDeviceUsageDistributionUserCountsCollectionPage getYammerDeviceUsageDistributionUserCounts = graphClient.reports()
    .getYammerDeviceUsageDistributionUserCounts("D7")
    .buildRequest()
    .get();

```