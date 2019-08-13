---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e37b5cc11959be0f69460bd7d262e36880aee6ce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320548"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsDeviceUsageDistributionUserCounts("D7")
    .buildRequest()
    .get();

```