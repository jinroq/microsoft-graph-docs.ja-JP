---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f9e475229d8d509c4ff72afbc2ad2b2ea0b78c42
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871826"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsDeviceUsageUserCountsCollectionPage getTeamsDeviceUsageUserCounts = graphClient.reports()
    .getTeamsDeviceUsageUserCounts('D7')
    .buildRequest()
    .get();

```