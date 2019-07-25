---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6502be681431ab6b6ebdd84f321dbee244ebe15f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870293"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecurityAction securityAction = graphClient.security().securityActions("{id}")
    .buildRequest()
    .get();

```