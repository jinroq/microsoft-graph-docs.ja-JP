---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5bdba3458af094a13e8583f716504b0a043fb5e1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893631"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveUsageStorage('D7')
    .buildRequest()
    .get();

```