---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 351b236ba470b5bcd60bbc732da7cdbd40564d32
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893544"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointActivityUserCounts('D7')
    .buildRequest()
    .get();

```