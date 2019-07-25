---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 3a869969d6e2f206175db3c6be3252d0c3b4293b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891873"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailActivityUserDetail('D7')
    .buildRequest()
    .get();

```