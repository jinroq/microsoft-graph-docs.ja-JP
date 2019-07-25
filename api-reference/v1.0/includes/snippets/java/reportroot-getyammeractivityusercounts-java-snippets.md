---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 309b4c58750ae33bb92165d80bf4cad1e1f720b7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891452"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerActivityUserCounts('D7')
    .buildRequest()
    .get();

```