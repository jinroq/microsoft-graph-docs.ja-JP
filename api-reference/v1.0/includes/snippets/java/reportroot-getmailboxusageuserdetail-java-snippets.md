---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 8b83d3ae78d3ecc7c75f73e38cb2b01f8b3cacb3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894436"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getMailboxUsageDetail('D7')
    .buildRequest()
    .get();

```