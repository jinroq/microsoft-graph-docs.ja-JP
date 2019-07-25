---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d77426d056e949caad6aba2f5a264647d2991392
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870315"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().securityActions("{id}")
    .cancelSecurityAction()
    .buildRequest()
    .post();

```