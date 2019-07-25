---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2d08b28212713b79e2aa263ce957f536a16899d0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871592"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerActivitySummaryCollectionPage getYammerActivityUserCounts = graphClient.reports()
    .getYammerActivityUserCounts('D7')
    .buildRequest()
    .get();

```