---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e83f15cd31c519bcb96d4dc21632b32e3955f771
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308511"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAppUsageUserCountsCollectionPage getEmailAppUsageUserCounts = graphClient.reports()
    .getEmailAppUsageUserCounts("D7")
    .buildRequest()
    .get();

```