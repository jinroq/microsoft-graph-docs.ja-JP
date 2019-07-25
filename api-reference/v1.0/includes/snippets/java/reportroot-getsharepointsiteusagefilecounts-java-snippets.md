---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9e438144ffbc6aef8ea04392c0cc527bc9263c3a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893435"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointSiteUsageFileCounts('D7')
    .buildRequest()
    .get();

```