---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1f068a239cf67fab12edec399fe16254f69cdd42
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885293"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsDeviceUsageDistributionUserCounts('D7')
    .buildRequest()
    .get();

```