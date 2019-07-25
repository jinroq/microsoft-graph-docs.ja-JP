---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b22cf3dd6e4cfb146809835d1c7f982964e8929e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892475"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessDeviceUsageDistributionUserCounts('D7')
    .buildRequest()
    .get();

```