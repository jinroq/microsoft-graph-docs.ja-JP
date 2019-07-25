---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 372eb9c2b67c399a8624a9a2aab19c6cdb6ac438
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886343"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailAppUsageUserDetail('D7')
    .buildRequest()
    .get();

```