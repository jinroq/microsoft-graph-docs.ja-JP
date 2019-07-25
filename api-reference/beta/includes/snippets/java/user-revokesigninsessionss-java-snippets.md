---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 224cb4e041c09e2d2f4c87cb73521da6c1e349b0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866758"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me()
    .revokeSignInSessions()
    .buildRequest()
    .post();

```