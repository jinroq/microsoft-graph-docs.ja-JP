---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 31292911d0e813f08a6cf382bb736cc460c586f1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886636"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsUserActivityUserDetail('D7')
    .buildRequest()
    .get();

```