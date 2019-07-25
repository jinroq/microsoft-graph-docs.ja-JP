---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d7139993fd6bb48e98cfda07a6de9a6eb92656e9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886657"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsUserActivityUserCounts('D7')
    .buildRequest()
    .get();

```