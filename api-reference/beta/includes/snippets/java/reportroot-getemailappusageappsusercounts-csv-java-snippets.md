---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2fc1f601fa5bc1fecd994d57736f25e45c86a9da
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308621"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAppUsageAppsUserCountsCollectionPage getEmailAppUsageAppsUserCounts = graphClient.reports()
    .getEmailAppUsageAppsUserCounts("D7")
    .buildRequest()
    .get();

```