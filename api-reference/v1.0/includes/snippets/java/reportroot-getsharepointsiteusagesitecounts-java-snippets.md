---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1ffd8ddcef0355f8af8c752a976332f4937891f4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357982"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointSiteUsageSiteCounts("D7")
    .buildRequest()
    .get();

```