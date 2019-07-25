---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 48601837f506ca419fc9f857f2ee66403d323855
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873906"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAppUsageUserCountsCollectionPage getEmailAppUsageUserCounts = graphClient.reports()
    .getEmailAppUsageUserCounts('D7')
    .buildRequest()
    .get();

```