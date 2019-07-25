---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 915c27ee384a680e3047d236d5ad8be914eadb7c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855598"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsUserActivityCounts('D7')
    .buildRequest()
    .get();

```